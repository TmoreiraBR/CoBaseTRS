# CoBaseTRS
CoBaseTRS, or Control Optimisation Baselines for Tidal Range Structures (TRS), is a collection of six optimisation baselines for the real-time (and upper bound estimate) control of TRS. All control routines consider two-way operation of TRS, with the goal of maximising power generation. For input data, 26 moths with ocean measurements and predictions from BODC, at the location of Mumbles station (Bristol Channel, UK) are provided. Ocean measurements (real data) contain the suffix "r", while tidal predictions contain the suffix "p". For further information regarding the starting/ending data of collection of each labbeled data (from 1 to 26), .txt files (without suffix) from BODC are also provided.

CoBaseTRS.ipynb is the main Jupyter notebook file in this repository. It can provide control optimisation estimates for any TRS design. As an example, it is currently setup with the design for the Swansea Bay Tidal Lagoon pathfinder project. By running the provided CoBaseTRS.ipynb, outputs for all optimisation methods are provided for a single month. The notebook contains instructions for installing required packages.

The optimisation baselines in CoBaseTRS are named CH, CHV, EHT, EHTV, EHN and EHNV. All methods are of the type "prediction-dependent" and "head-controlled", i.e. (i) they utilise tide signal forecasts for (ii) acquiring best operational water heads for operating TRS.

CH, EHT and EHN methods were developed based on the work of [1, 2], and named as "classic" approaches. The remaining CHV, EHTV and EHNV methods consider a novel "variant" operation of TRS, with independent sluice operation (inspired by the work of [3, 4]) and first published in [5].

[1]: Ahmadian, Reza, et al. "Optimisation of tidal range schemes." Proceedings of the 12th European Wave and Tidal Energy Conference. 2017.
[2]: Xue, Jingjing, Reza Ahmadian, and Roger A. Falconer. "Optimising the operation of tidal range schemes." Energies 12.15 (2019): 2870.
[3]: Baker, Clive. "Tidal power." Energy Policy 19.8 (1991): 792-797.
[4]: Angeloudis, Athanasios, et al. "Optimising tidal range power plant operation." Applied energy 212 (2018): 680-690.
[5]: Moreira, Túlio Marcondes, et al. "Prediction-free, real-time flexible control of tidal lagoons through Proximal Policy Optimisation: A case study for the Swansea Lagoon." Ocean Engineering 247 (2022): 110657.

**This study uses data from the National Tidal and Sea Level Facility, provided by the British Oceanographic Data Centre (BODC) and funded by the Environment Agency.**
