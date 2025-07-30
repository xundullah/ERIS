# Energy-Resilient Integrated System (ERIS) for Cellular Base Stations

## Overview
This repository contains the implementation and documentation of the **Energy-Resilient Integrated System (ERIS)**, a predictive, rule-based energy dispatch framework designed to enhance the power resilience of 5G cellular base stations (CBSs) under extreme weather conditions. ERIS integrates renewable energy sources (RES) such as photovoltaic (PV) panels and wind turbines (WT), alongside energy storage systems (ESS) and grid power, to ensure uninterrupted CBS operation during severe weather events. The system employs a centralized, event-aware control strategy segmented into pre-event, severe-event, and post-event phases, leveraging real-time meteorological data for adaptive power flow management.

The framework was developed as part of research supported by the **Connectivity Innovation Network (CIN)**, Australia, under the CIN PhD Scholarship Program (Org: 325720, Activity: 1033584). It was validated through simulations using real-world meteorological and load data from Wollongong, New South Wales, during a severe storm event in January 2025.

## Repository Contents


## Key Features
The ERIS framework offers the following contributions:
1. **Integrated System Architecture**: Combines PV, WT, ESS, and grid power to support macro and micro 5G CBSs under centralized control.
2. **Analytical Models**: Component-wise models for CBS load demand, PV and WT generation, and ESS dynamics, derived from real-world data.
3. **Event-Aware Dispatcher**: A rule-based algorithm that adjusts power flows based on pre-event, severe-event, and post-event phases, triggered by localized meteorological forecasts.
4. **Simulation-Based Validation**: Demonstrates a 66.4% reduction in grid energy consumption while maintaining uninterrupted CBS operation during a 10-day simulation, including a three-day severe storm event.


## Results
The ERIS framework was validated through a 10-day simulation (January 10–20, 2025) in Wollongong, NSW, covering a three-day severe storm event. Key outcomes include:
- **Grid Energy Reduction**: Achieved a 66.4% reduction in grid energy consumption compared to a baseline without RES.
- **Resilient Operation**: Maintained continuous CBS operation with ESS SoC ranging from 89.3% (pre-storm) to 60.3% (post-storm).
- **Efficient Resource Use**: Harvested 1943 kWh of renewable energy, with 82 kWh exported to the grid, resulting in a net import of 503 kWh.

Detailed results, including time-series plots of power demand, renewable generation, grid interaction, and ESS behavior, are presented in the paper and can be reproduced using the provided simulation code.

## Future Work
Future enhancements to the ERIS framework include:
- Replacing external meteorological forecasts with on-site sensor data and historical patterns for localized weather prediction.
- Implementing deep reinforcement learning for adaptive, closed-loop control to optimize dispatch decisions under varying conditions.
- Extending the framework to support additional RES types (e.g., hydrogen-based systems) and larger-scale CBS networks.

## Citation
If you use this work in your research, please cite the following paper:
> R. B. Mofidul, M. J. Hossain, and M. M. Alam, "Sustainable Power Provisioning for Cellular Sites: Adaptive Control Under Extreme Weather," *2025 IEEE International Conference on Energy Technologies for Future Grids*, Wollongong, Australia, December 7–11, 2025.

BibTeX entry:
```bibtex
@inproceedings{mofidul2025sustainable,
  author={Mofidul, Raihan Bin and Hossain, M. J. and Alam, Md. Morshed},
  title={Sustainable Power Provisioning for Cellular Sites: Adaptive Control Under Extreme Weather},
  booktitle={2025 IEEE International Conference on Energy Technologies for Future Grids},
  address={Wollongong, Australia},
  month={December},
  year={2025},
  pages={1--8},
  publisher={IEEE}
}
```

## Acknowledgments
This research was supported by the **Connectivity Innovation Network (CIN)**, Australia, under the CIN PhD Scholarship Program (Org: 325720, Activity: 1033584), titled "Data-driven design and management of shared energy resources to improve power supply resilience in communication networks." The work was conducted under the supervision of Prof. Dr. M. J. Hossain at the University of Technology Sydney (UTS). For more details, visit the [CIN Scholarship Recipients page](https://www.connectivityinnovationnetwork.com/scholarships/).

## Contact
For inquiries, please contact:
- **Raihan Bin Mofidul**: [raihan.binmofidul@student.uts.edu.au](mailto:raihan.binmofidul@student.uts.edu.au)
- **M. J. Hossain**: [jahangir.hossain@uts.edu.au](mailto:jahangir.hossain@uts.edu.au)
- **Md. Morshed Alam**: [mmorshed@ieee.org](mailto:mmorshed@ieee.org)

## License
This repository is licensed under the [License](LICENSE). Users are free to use, modify, and distribute the code and documentation, provided proper attribution is given.
