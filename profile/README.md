# StrangeLand

**Open-source tools for studying how people interact with each other and with robots and automated vehicles: several people at once, in the lab and in real places.**

StrangeLand puts several participants (drivers, pedestrians, cyclists, operators of robots) into the same virtual scene over a network, so they respond to each other in real time. It runs on consumer VR headsets and ordinary PCs, and a full setup fits in checked luggage, which is why research groups on three continents have been able to run the same studies in different places.

🌐 **Project site:** [strangelandcommons.org](https://strangelandcommons.org) · 📖 **Docs:** [strangeland.io](https://strangeland.io) · ✉️ hello@strangelandcommons.org

---

## Start here

| If you want to… | Use |
|---|---|
| Build a new multi-person study in Unity | [StrangeLandPackage](https://github.com/Strange-Land/StrangeLandPackage) (core), plus [strangeland.steering](https://github.com/Strange-Land/strangeland.steering) and [strangeland.vehicle](https://github.com/Strange-Land/strangeland.vehicle) |
| Connect a steering wheel, pedals or other driving input | [strangeland.steering](https://github.com/Strange-Land/strangeland.steering) |
| Add a ready-to-drive vehicle to a scene | [strangeland.vehicle](https://github.com/Strange-Land/strangeland.vehicle) |
| Run pedestrian–driver studies with a portable setup | [Grokwalk](https://github.com/Strange-Land/Grokwalk) |
| Record a session and replay it from any viewpoint | [Rerun](https://github.com/Strange-Land/Rerun) |
| Reproduce or extend an earlier study | [StrangeLand-Base](https://github.com/Strange-Land/StrangeLand-Base) (legacy, see below) |

New projects should start from the **packages**: install them through Unity's Package Manager and import the samples. Setup guides live in [Docs-ReadMe](https://github.com/Strange-Land/Docs-ReadMe) and will move to [strangeland.io](https://strangeland.io).

**Requirements:** Unity [version], Windows PC with a VR-capable GPU, [supported headsets, e.g. Meta Quest 2/Pro/3]. Steering wheels supported through the steering package (Logitech examples included).

---

## Repositories

**Core packages (current)**
- **[StrangeLandPackage](https://github.com/Strange-Land/StrangeLandPackage):** networking, participant and scenario management, data logging. Samples are available in the Package Manager.
- **[strangeland.steering](https://github.com/Strange-Land/strangeland.steering):** a hardware abstraction layer for steering wheels and pedals. `SteeringWheelManager` exposes normalized steering, throttle, brake and controls, so vehicle code stays independent of any one SDK. Add it to your `GameManagement` scene.
- **[strangeland.vehicle](https://github.com/Strange-Land/strangeland.vehicle):** a reference vehicle with interior, mirrors and audio, wired to `SteeringWheelManager` and the spawning system.

**Companion tools**
- **[Rerun](https://github.com/Strange-Land/Rerun):** records every moving actor in a scene and plays sessions back from any perspective, for coding and analyzing interactions.
- **[Grokwalk](https://github.com/Strange-Land/Grokwalk):** a portable configuration for studying driver–pedestrian interaction.
- **[StrangeHarbour](https://github.com/Strange-Land/StrangeHarbour):** [one-line description].

**Documentation and site**
- **[Docs-ReadMe](https://github.com/Strange-Land/Docs-ReadMe):** guides and the [technical roadmap](https://github.com/Strange-Land/Docs-ReadMe/wiki/Technical-Improvments).
- **[strange-land.github.io](https://github.com/Strange-Land/strange-land.github.io):** source for the documentation site.

**Legacy**
- **[StrangeLand-Base](https://github.com/Strange-Land/StrangeLand-Base)** and **[Core](https://github.com/Strange-Land/Core)**: the original monolithic simulator, used in published studies. Kept for reproducing earlier work; new projects should use the packages.
- The simulator's original history and issue tracker remain at [FAR-Lab/CrossCulturalDriving](https://github.com/FAR-Lab/CrossCulturalDriving).

**Community forks**
- **[humanFUEL-StrangeLand](https://github.com/Strange-Land/humanFUEL-StrangeLand):** a fork maintained for pedestrian studies. Many groups keep their own forks; see *Contributing* for how to share extensions back.

---

## What's next: StrangeLand Commons

StrangeLand is becoming **StrangeLand Commons**: one maintained platform that labs and companies can set up without help from its developers. Planned work includes connections to [CARLA](https://carla.org), Gazebo and ROS 2 so the same study can run with live people and with software agents; mixed reality for running lab studies in real places; a shared format for describing multi-party scenarios; and a shared dataset of recorded interactions.

---

## Contributing

We welcome bug reports, feature requests and extensions, including work that started in your own fork.
- **Questions and bugs:** open an issue in the relevant repository.
- **Extensions:** if you've built something in a fork (a new vehicle, robot, sensor or study type), open a pull request against the package it extends, or an issue describing it, and we'll help bring it into the shared code.
- See [CONTRIBUTING.md](https://github.com/Strange-Land/.github/blob/main/CONTRIBUTING.md) for details.

All code is released under the **MIT license**.

---

## Citing StrangeLand

If you use StrangeLand in your research, please cite:

> D. Goedicke, C. Zolkov, N. Friedman, T. Wise, A. Parush and W. Ju, "Strangers in a Strange Land: New Experimental System for Understanding Driving Culture Using VR," *IEEE Transactions on Vehicular Technology*, vol. 71, no. 4, pp. 3399–3413, 2022. [doi:10.1109/TVT.2022.3152611](https://doi.org/10.1109/TVT.2022.3152611)

```bibtex
@article{goedicke2022strangers,
  title   = {Strangers in a Strange Land: New Experimental System for Understanding Driving Culture Using {VR}},
  author  = {Goedicke, David and Zolkov, Carmel and Friedman, Natalie and Wise, Talia and Parush, Avi and Ju, Wendy},
  journal = {IEEE Transactions on Vehicular Technology},
  volume  = {71},
  number  = {4},
  pages   = {3399--3413},
  year    = {2022},
  doi     = {10.1109/TVT.2022.3152611}
}
```

If you use Rerun, please also cite *ReRun: Enabling Multi-Perspective Analysis of Driving Interaction in VR* (HRI 2023, [doi:10.1145/3568294.3580211](https://doi.org/10.1145/3568294.3580211)).

---

## History

StrangeLand began at Cornell Tech and the Technion in Israel, to compare how drivers in different countries negotiate the same intersection. It has since grown to cover pedestrians, cyclists, robots, flying vehicles and on-road studies, and is used by research groups and industry researchers in the United States, Europe and Asia.
