# The electrocardiogram (ECG) based biometric identification
基於心電圖 (ECG) 的個人身份識別
- This project is the Graduation Project / Final Year Project (FYP) of Department of Computer and Information Science, Faculty of Science and Technology, University of Macau. 

## Abstract
- Biometric identification mainly uses the inherent physiological and behavioural characteristics of the human body to identify individuals. It includes fingerprint, face, iris, handwriting, sound, gait etc. In this case, we build a low-cost biometrics identification method to give a new choice to the identification technical area. We introduce the ECG biometric identification because it is new, low-cost and keep the tester is alive when it is testing.
- 個人生物及身份特徵識別主要是利用人體固有的生理和行為特徵來識別個體。它包括指紋，面部，虹膜，筆跡，聲音，步態等。在這種情況下，我們正在構建一種低成本的生物特徵識別方法，以便為識別技術領域提供新的選擇。我們會選擇使用用心電圖 (ECG) 生物識別技術，因為它是一種新穎的低成本技術，而且可在測試時保證測試者在存活的狀態。

## Dataset used for model testing training
* ECG-ID Database v1.0.0: https://physionet.org/content/ecgiddb/1.0.0/

## Environment Requirement
* OS: Windows / Linux / Mac OS *(This project developed in macOS Catalina 10.15.3 & Ubuntu 18.04 LTS)*
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
  - Check the Serial Monitor and Serial Plotter in Arduino IDE to see the signal value and graph respectively
  - Collect the signal in Serial Potter and do the further process

- Training Model and GUI application (*Python*):
  - Open the program with *Jupyter Notebook* or *Google Colaboratory*
  - Check the paths in program
  - If everything is fine, click "Kernel -> Restart and Run All"
  - **For GUI identification application**, change and check the port of Arduino UNO everytime.

## Contact
* Oscar, Kuan Ka Meng (macauoscar@gmail.com)
