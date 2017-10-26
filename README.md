# cwru_davinci_hardware
[![Build Status](https://travis-ci.com/cwru-robotics/cwru_davinci_hardware.svg?token=YmHMxBbcdppbMMkZWTut&branch=master)](https://travis-ci.com/cwru-robotics/cwru_davinci_hardware)

This package stores hardware specific information as well as the documenting launch and control procedures for the the da Vinci Reseach Kit located at Case Western Reserve U. This package contains a copy of the dvrk consol controller which was originally released by JHU. The current JHU code can be found [here](https://github.com/jhu-dvrk/dvrk-ros). This package is licensed under the GPLv3+ license except where the original source is from JHU's dvrk-ros library.

The dependency list is maintained by the presence of dependencies.rosinstall as well as the package.xml file.

# Included Launch Files

The following launch files are included for launching the hardware.
1. teleop_default_defaul.launch: rviz:=True will launch an RVIZ display of the robot. There is no RVIZ by default.


# Alternative Hardware target

If one wishes to modify this package to use a different da Vinci platform, then they should perform the following steps...

1. Make a new folder inside the share directory (i.e. <institution>_dvrk) and place the xml calibration files inside of it accordingly.
2. populate the calibration files (i.e. MTML-<serial>.xml)
3. create a *.json file that calls the calibration files
4. modify (or copy) the launch file accordingly.



