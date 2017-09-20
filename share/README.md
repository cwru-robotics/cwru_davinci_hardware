# cwru_davinci_hardware/share

The share directory of the cwru_davinci_hardware package contains the *.json files which are used to store robot hardware parameters.

The .json file extension is a holdover from how the files are defined for use with CISST as developed by JHU.

The folder are used as follows:

1. cwru_dvrk : contains files specific to the davinci hardware instance which exists inside the Case Western Reserve University MeRCIS Lab.
2. kinematics : contains the DH style DH parameters of the davinci hardware. This is common accross hardware instances.
3. pid : contains the control 

## hardware localization

If one were to set up the hardware to use with a robot distinct from the one Case Western, then they would have to do the following: 

1. make a new folder (i.e. University_dvrk).
2. generate the xml calibration files, [using these directions](https://github.com/jhu-dvrk/sawIntuitiveResearchKit/wiki/XMLConfig) then [these](https://github.com/jhu-dvrk/sawIntuitiveResearchKit/wiki/Calibration).
3. create a config file similar to cwru_dvrk/teleop_default_default.json which loads the hardware specific calibration, kinematics, and control gains.


## *.json file format

The *.json file format ([defined here](https://en.wikipedia.org/wiki/JSON)) is heavily used for defining robot control parameters.