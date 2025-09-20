# 5.-Design-and-Simulation-of-step-down-chopper
## AIM
To design, simulate and analyse a step down chopper using MATLAB Simulink.
## APPARATUS REQUIRED
	MATLAB
## PROCEDURE
1.	Open MATLAB and click on the icon for SIMULINK as shown below
 <img width="522" height="376" alt="image" src="https://github.com/user-attachments/assets/545a1702-442f-4f55-94db-225ccabc88ff" />

Another way is to open is through START icon of MATLAB Start ⇒ Simulink ⇒ Library  browser. 

2.	Click on NEW MODEL or go to FILE ⇒ NEW ⇒ MODEL and a new blank model is created as shown below
 <img width="572" height="382" alt="image" src="https://github.com/user-attachments/assets/1409107c-f0df-4f4f-813a-9267f029553b" />

3.	After creating a blank model you need to open the SIMULINK component storeroom/library by going to View ⇒ Library Browser. Select SIMPOWER SYSTEMS then select Power Electronics library and by right clicking on MOSFET and click on add to the model will add the MOSFET in the blank model. Alternatively you can drag the component directly in the model page as shown below
 <img width="940" height="361" alt="image" src="https://github.com/user-attachments/assets/b3e2aed8-b30d-48f6-aa5a-fdf5e0bc04a5" />

4.	Similarly go to ELECTRICAL SOURCES ⇒ AC Voltage Source and add it to the model. Select Elements and select “SERIES RLC BRANCH” and add it to the model. Simulink do not perform simulation unless and until a measurement block is present in a system. Since we need to measure the input and output voltages and the load current. To add them select Measurement in SIMPOWER SYSTEMS and then add current measurement and voltage measurement blocks to the model. Oscilloscope is not included in SIMPOWER SYSTEMS and is present in the top most block of the left column that is SIMULINK ⇒ Sinks ⇒ Scope. Also add PWM generator from sourced. We can join various blocks by clicking on their edges and then drag the wire till the other connection terminal.
5.	Construct the circuit by joining them together in the form as given below
 <img width="940" height="469" alt="image" src="https://github.com/user-attachments/assets/f76a4b1b-f842-432e-a0ae-695420974775" />

6.	Double click on series RLC branch, Select the Branch type as R and set the values for R.
7.	Double click on PWM generator, set the parameter as per the requirement.
 <img width="516" height="452" alt="image" src="https://github.com/user-attachments/assets/1fad018a-d7c8-4446-8049-9e47cd2e043a" />

8.	Before running the simulation, we have to configure the parameters. Go to Simulation ⇒ Configuration parameters as shown
 <img width="542" height="399" alt="image" src="https://github.com/user-attachments/assets/ac105b60-7369-4f34-bc8c-87b2c1980a08" />

9.	Select the ode23tb (Stiff/TR-BDF2) or ode15s (Stiff/NDS) or any suitable solver as
shown below 
 <img width="566" height="401" alt="image" src="https://github.com/user-attachments/assets/82ee7c4a-2edd-443d-b4ec-66a36cffc6e9" />

10.	Start the simulation and Double click on scope and observe the graphs.

 
## Exercise 1
Design a step down chopper for the following specification
Specification
Input Voltage (Vin)=12V
Output Voltage (Vout) = 5V
Switching Frequency (Fs) = 25 KHz
Voltage Ripple (∆V) = 20mV
Current Ripple (∆I) = 0.1A

## Exercise 2
Design a step down chopper for the following specification
Specification
Input Voltage (Vin)=48V
Output Voltage (Vout) = 12V
Switching Frequency (Fs) = 25 KHz
Voltage Ripple (Delta V) = 20mV
Current Ripple (Delta I) = 0.1A

## Simulation

<img width="1920" height="759" alt="PEEXP5 CD" src="https://github.com/user-attachments/assets/c39e6a78-dbad-4a40-83bf-b5b9228bba80" />

## Output

<img width="1920" height="843" alt="PEEXP5 WF" src="https://github.com/user-attachments/assets/cb918a9a-a382-4404-a9d6-5bb9f2c4bcab" />

## Result
STEP DOWN CHOPPER IS DESIGNED AND SIMULATED IN MATLAB SUCCESSFULLY.
