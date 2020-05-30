# The electrocardiogram (ECG) based biometric identification
基於心電圖 (ECG) 的個人身份識別
- This project is the Graduation Project / Final Year Project (FYP) of Department of Computer and Information Science, Faculty of Science and Technology, University of Macau. 

## Abstract

## Dataset of pre-training
* ECG-ID Database v1.0.0: https://physionet.org/content/ecgiddb/1.0.0/

## Environment Requirement
* OS: Windows / Linux / Mac OS
* Python Version: Python 3 *(Python 3.7.4 is recommanded)*
* Others:
  - Arduino IDE *(Version 1.8.12 is recommanded)*
  
## Hardware Requirement
* Computer with required environment
* Arduino UNO R3 (with USB cable)
* AD8232 Heart Beat / ECG Collecting Shield (with sensors/electrodes)

## Python 3 library installation
* Library using pip to install:
  - jupyter
  - wfdb
  - pandas
  - numpy
  - glob2
  - tensorflow
  - matplotlib
  - math3
  - scikit-learn
  - joblib
  - pyserial
  - tkinter
* Windows command: <code>py -m pip install [library]</code>
* Linux & Mac OS command: <code>pip install [library]</code>

### For problem of *tkinter* installation problem in Linux:
<code>sudo apt-get install python3-tk</code>

### For problem of serial port connection in Linux:
<code>sudo chmod 666 [port]</code>

### Open ipynb file
* Windows: <code>py -m jupyter notebook</code>
* Linux & Mac OS: <code>jupyter notebook</code>

### Stop running Jupyter notebook
* Windows: <code>py -m jupyter notebook stop</code>
* Linux & Mac OS: <code>jupyter notebook stop</code>

## Open Program
- Arduino (Open with *Arduino IDE*):
  - <code>/src/arduino/ECG_arduino/ECG_arduino.ino</code>
- Python (Open with *Jupyter Notebook* or *Google Colaboratory*)
  - Training Model: <code>/src/python/ECG_Prediction_SVM.ipynb</code>
  - GUI Identification Application: <code>/src/python/ECG_GUI_App.ipynb</code>

## Start and Running Program
- Collecting ECG Signal (*Arduino*): 
  - Connect Arduino UNO R3 with AD8232 Heart Beat / ECG Collecting Shield to Computer with Arduino IDE
  - Check the USB port is available
  - Paste the sensors/electrodes on user's body
  - Check the Serial Potter and Serial Monitor in Arduino IDE to see the signal value and graph respectively
  - Collect the signal in Serial Potter and do the further process

- Training Model and GUI application (*Python*):
  - Open the program with *Jupyter Notebook* or *Google Colaboratory*
  - Check the paths in program
  - If everything is fine, click "Kernel -> Restart and Run All"

## Contact
* Oscar, Kuan Ka Meng
* Elaine, Guo Yan Jia
