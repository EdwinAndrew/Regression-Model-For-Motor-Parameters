# Regression Model Between Electric Motor Parameters

## Context

The data set comprises several sensor data collected from a permanent magnet synchronous motor (PMSM) deployed on a test bench. The PMSM represents a german OEM's prototype model. Test bench measurements were collected by the LEA department at Paderborn University. 
This data set is mildly anonymized.

## Content

All recordings are sampled at 2 Hz. The data set consists of multiple measurement sessions, which can be distinguished from each other by column "profile_id". A measurement session can be between one and six hours long.

The motor is excited by hand-designed driving cycles denoting a reference motor speed and a reference torque.
Currents in d/q-coordinates (columns "id" and iq") and voltages in d/q-coordinates (columns "ud" and "uq") are a result of a standard control strategy trying to follow the reference speed and torque.
Columns "motor_speed" and "torque" are the resulting quantities achieved by that strategy, derived from set currents and voltages.

Most driving cycles denote random walks in the speed-torque-plane in order to imitate real world driving cycles to a more accurate degree than constant excitations and ramp-ups and -downs would.

## Inspiration

The most interesting target features are rotor temperature ("pm"), stator temperatures ("stator_*") and torque.
Especially rotor temperature and torque are not reliably and economically measurable in a commercial vehicle.

Being able to have strong estimators for the rotor temperature helps the automotive industry to manufacture motors with less material and enables control strategies to utilize the motor to its maximum capability.
A precise torque estimate leads to more accurate and adequate control of the motor, reducing power losses and eventually heat build-up.

## References
- [Kaggle](https://www.kaggle.com/wkirgsn/electric-motor-temperature)

## License
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

## Sections 
- Basic Linear Regression
- Multiple Linear Regression
- Principle Component Regression
- KNN Regression
- Polynomial Regression

## Sample Data Visualizations
#### Heat Map
![Heat Map](https://user-images.githubusercontent.com/48691226/100554519-24791c00-3263-11eb-9187-7b9b2c1ed943.png)
#### PCR Model Tuning 
![PCR Model Tuning](https://user-images.githubusercontent.com/48691226/100554527-28a53980-3263-11eb-9913-1715759c8eac.png)
#### Residual Error for Training and Test Data
![Residual Error](https://user-images.githubusercontent.com/48691226/100554495-fa275e80-3262-11eb-8f79-15bf4a7f12fa.png)




