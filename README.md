# OpenSense_matlab_scripts

*for now the myIMUMappings.xml and IMUDataConversion_GH.m are not used

INPUTS: prepare a folder with <br />
- *.sto file <br />
- *.xml file <br />
- model_scaled.osim <br />
- matlab scripts

These following steps refer to the OpenSense guide (Step 3 and 4):<br />

Step0: open and prepare the .xml file (see OpenSense guide - black windows)<br />
      - use -z as forward <br />
      - -pi/2, 0, 0 as rotation <br />
      - pelvis as base imu <br />

Step1: run OpenSense_CalibrateModel_GH.m (see comments inside the script)<br />

OUPUT: calibrated_model.osim<br />

Step2: run OpenSense_OrientationTracking_GH.m (see comments inside the script)<br />

OUTPUTS: IK.mot<br />

Step3: open OpenSim 4.1 and load model (calibrated_model.osim) and load motion (IK.mot)<br />
