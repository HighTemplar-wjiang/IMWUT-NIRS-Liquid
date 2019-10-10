# IMWUT-NIRS-Liquid
This is the Source code repository for IMWUT paper:
*Probing Sucrose Contents in Everyday Drinks Using Miniaturized Near-Infrared Spectroscopy Scanners*
(to appear)

We show a generic and mobile method to estimate concentration level for a specific ingredient in a solution (*e.g.*, sugar concentration in soft-drinks), identify liquids (*e.g.*, discriminate different drinks or alcohols), or even detect counterfeit liquids (*e.g.*, detect counterfeit perfume or alcohols), etc. 

## What's included? 
1. Hardware schemetics.

1. Python library with source code for NIRScan Nano that works for Linux, Mac and Raspberry Pi.

1. Example Python code for training regression models.

1. Example Python code for training classification models.

## Dependencies
**Hardware**
- [Texas Instruments NIRScan Nano](http://www.ti.com/tool/DLPNIRNANOEVM).
- Makerbot Replicator Z18 or equivalent (recommended to use a 3D printing service for minimal cost).

*(Optional for standalone mode)*

- Raspberry Pi A+.
- Adafruit 2.8-inch PiTFT.
- Li-Po battery.
- PowerBoost 1000C or equivalent.

**For compiling the Python library**

Please refer to [this repository](https://github.com/HighTemplar-wjiang/NIRScanner-Python).

**For running the Python scripts**
- Python3
- Numpy
- Matplotlib 
- Seaborn
- Scikit-learn
- Pandas
- Jupyter Notebook or Jupyter Lab (recommended)

## Quick start
1. In your console, using the *cd* command to change your current path to this repository. 
1. Run *jupyter notebook* or *jupyter lab*.
1. In Jupyter open the *quick_start.ipynb* file.
1. Execute the cells to train/test/export your models using your data. 

## Running as a standalone device
1. Assemble the device as shown in the paper. 
1. Copy the *src/standalone/* folder to Raspberry Pi. 
1. Copy your sklearn model file into *standalone/model/regressor/* folder for regression tasks, or *standalone/model/classifier* for classification tasks. 
1. Run the *main.py* script. 

## Tips for developing your applications
1. Follow the protocol and collect your data as described in the paper.
1. Controlling the optical path is the key when you re-design a 3D-print case for your application.
1. Calibrition may be critical to aqcuire consistent results across different conditions.
1. Try different filtering methods. 
1. Keep calm and cite my paper ;-)

## Contact
Please send me an email if you have any question.

weiweijiangcn\[at\]gmail.com
