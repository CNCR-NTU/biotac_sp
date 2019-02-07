# Biotac SP

This is repository for hosting the Biotac SP sensors sofware released under the lgpl3.0 license.

# Requirements

## Hardware
* 3x Biotac SP sensors
* Biotac Board
* uUSB power cable for connecting the Biotac board
* Cheetah SPI host
* USB-B cable.
* Host pc

## Software
* Ubuntu Linux 18.04 LTS

# Installation procedure:
## Step 1: Connect the equipment 
Figure 1 shows the configuration setup

![](https://github.com/pedrombmachado/biotac_sp/blob/master/doc/Biotac.png)

Figure 1: Biotac setup
  
## Step 2: Update the OS and install base packets

```
$ sudo apt update & sudo apt upgrade -y & sudo apt dist-upgrade -y & sudo apt autoremove -y & sudo apt autoclean -y
$ sudo apt install build-essential git
```

## Step 3: clone the repository
```
$ cd ~
$ git clone git@gitlab.com:CNCR-NTU/biotac_sp_sensors.git
```

## Step 4: install the drivers
```
$ cd biotac_sp_sensors
$ ./installCheetahDriver.sh
```

## Step 5: compile and run
```
$ make
$ bin/biotac_sp
```

# Support
Pedro Machado <pedro.baptistamachado@ntu.ac.uk>
