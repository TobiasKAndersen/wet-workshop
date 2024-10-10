## The **Water Ecosystems Tool (WET)** model workshop

On this page, you will find materials, lectures, exercises and tutorials to train and support your application of Water Ecosystems Tool (WET). This workshop trains participants in the theory and practical application of WET coupled to the 1D hydrodynamic model General Ocean Turbulence Model (GOTM). The workshop covers the theory behind as well as model development of the lake models PCLake and WET. Through combined lectures and hands-on exercises on participants own computers, participants will learn how to
*	Set-up a GOTM-WET lake model via the QGIS interface QWET
*	Manual calibration and scenario executions with GOTM-WET models
*	Auto-calibration and sensitivity analysis of WET models with parsac
*	Compile GOTM-FABM-WET executable from source code
*	Contribute to the development of WET modules

The software used has been developed for Windows computers, and participants therefore need a Windows computer to be able to follow the hands-on exercise.

The workshop takes place on 14 to 16 October 2023 at NIGLAS, Nanjing, China.

## Workshop materials
To participate in the hands-on part of the workshop, you will need to have a working version of QGIS and the graphical user interface QWET. If you are a Mac user, we highly recommend you apply a windows-partition on your system, as the QWET installer is only available in windows format.

On day 1, we provide video tutorials on setting up, calibrating and running scenarios of GOTM-WET models with QWET. We therefore recommend bringing a headset, so you can work on the exercises while viewing the video tutorials by yourself.

**QGIS**

To run QWET you need to install QGIS3 64 bit version 3.16 or newer (available here: www.qgis.org). We recommend you install QGIS3 64 bit version 3.22 (QWET is currently tested up to version 3.36).

**QWET**

QWET is an open source QGIS plugin for application and user adaptation of the Water Ecosystems Tool (WET). The QWET installer and the QWET source code is available through here in the _Materials_ folder. The newest release of QWET (OCtober 2024, version 3.6) is compatible with the latest long term release of QGIS (version 3.34). Please read the download instructions and watch the associated video tutorial on how to download the software at: https://projects.au.dk/wet/resources

_GOTM-WET executables_

GOTM-WET executables are available to users with QWET download and installation. For users not interested in using QWET, GOTM-WET v2.1 executable for 64-bit Windows can be downloaded on the [WET Zenodo repository](https://doi.org/10.5281/zenodo.13841743).

**Case study data for Shahe Reservoir**

For our case study, we will work with the Chinese Shahe reservoir. Yiu can access to the case study folder including files to configure a GOTM-WET model to Shahe Reservoir with QWET with lake specific hypsography and inflow and weather forcing as well as in-lake observations and files with calibrated parameters in the _Materials_ folder.

**PyNCView**

To visualize model output with contour plots, we recommend using the software PyNCView.  We recommend you download PyNCView in Python via “pip install pyncview”. You can also download an installer (for Windows) at this page [pyncview-0.99.9.msi](https://github.com/BoldingBruggeman/pyncview/releases) (under Assets).

**parsac**

parsac is a Python-based tool for sensitivity analysis and auto-calibration in parallel developed by Bolding&Bruggeman. It is designed for analysis of models that take significant time to run. To download parsac, you will need a Python working environment (we recommend using Python3 via [Anaconda distribution](https://www.anaconda.com/download/) ) and can install via Python pip: “pip install parsac –user”. parsac requires the Python package Parallel Python to parallelize the auto-calibration process and the Python package SALIb for sensitivity analysis. For more details on parsac and package dependencies look into the tutorials on auto-calibration and sensitivity analysis. You can also find more information on [parsac's Github page] (https://github.com/BoldingBruggeman/parsac).

If you have problems installing the required software or downloading the case study, you are welcome to contact us by posting your challenge on the Issues board. 

## More resources
**Water Ecosystems Tool (WET)**

WET is a further development of FABM-PCLake by Hu et al., at Aarhus University, Denmark. Key features originate from the PCLake aquatic ecosystem model by Janse and van Liere (1995), but key features and inspiration from CAEDYM and Ecopath/Ecosim has also been implemented.  WET can describe interactions between multiple trophic levels and abiotic nutrient dynamics in both the water column and the sediment. The model accounts for the dynamics of dry weight, nitrogen, phosphorous, silica and oxygen, and features bottom-shear-dependent resuspension, as well as two different light-limitation functions for phytoplankton. WET is also implemented within the FABM framework, allowing the model to be coupled to various physical driver models, e.g. GOTM (1D, Burchard et al., 1999) or GETM (3D, e.g. Stips et al., 2004), without changing any of the model code. 
For introduction to WET, we refer you to the scientific articles:

Schnedler-Meyer, N. A., Andersen, T. K., Hu, F. R. S., Bolding, K., Nielsen, A., & Trolle, D. (2022) Water Ecosystems Tool (WET) 1.0 – a new generation of flexible aquatic ecosystem model. [Geoscientific Model Development](https://doi.org/10.5194/gmd-15-3861-2022)

Schnedler-Meyer, N. A., & Andersen, T. K. (2024) Dining in danger: Resolving adaptive fish behavior increases realism of modeled ecosystem dynamics. [Ecology and Evolution](https://doi.org/10.1002/ECE3.70020)

**General Ocean Turbulence Model (GOTM)**

Most commonly WET is coupled to the lake branch of 1D hydrodynamic model GOTM (source code available at https://gitlab.com/wateritech-public/waterecosystemstool/gotm). For details on lake branch GOTM, see the models Gitlab page. For more information on GOTM in general, check out https://gotm.net/portfolio/. 

For a brief description of GOTM and how it compares to other 1D hydrodynamic models, we recommend
Feldbauer, J., Mesman, J.P., Andersen, T.K., Ladwig, R. (under review) Learning from a large-scale calibration effort of multiple lake models. [Preprint egusphere-2024-2447](https://doi.org/10.5194/egusphere-2024-2447)

**Framework of Aquatic Biogeochemical Models (FABM)**

The Framework for Aquatic Biogeochemical Models (FABM, developed by Bolding & Bruggeman) allows coupling a biogeochemical model to a wide variety of hydrodynamic models in 0D, 1D, 2D or 3D, without changing any model code, and encourages and supports modularization of ecosystem models. For more details, we refer you to [FABMS wiki page] (https://github.com/fabm-model/fabm/wiki).

**Model study on the Shahe Reservoir**

You can find more information on the model study of Shahe Reservoir, which this workshop is based around, in the paper

Cui, Y., Zhu, G., Li, H., Luo, L., Cheng, X., Jin, Y., & Trolle, D. (2016). Modeling the response of phytoplankton to reduced external nutrient load in a subtropical Chinese reservoir using DYRESM-CAEDYM. [Lake and Reservoir Management](https://doi.org/10.1080/10402381.2015.1136365), 32(2), 146–157. 
