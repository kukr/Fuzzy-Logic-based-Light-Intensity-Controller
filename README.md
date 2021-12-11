# Fuzzy-Logic-based-Light-Intensity-Controller

<h2>Introduction</h2>
Home automation involves control or automation of home, housework or household activity. Home automation may include centralized control of lighting, HVAC (heating, ventilation and air conditioning), appliances, security locks of gates and doors and other systems, to provide improved convenience, comfort, energy efficiency and security.

![](https://github.com/kukr/Fuzzy-Logic-based-Light-Intensity-Controller/blob/master/assets/home-automation.png)

Every home automation system consists of a controller which is the central part of the system. The controller takes the input from sensors and according to the input gives signal to actuators which are fixed to the devices to be controlled.
Fuzzy logic is a form of many-valued logic in which the truth values of variables may be any real number between 0 and 1. By contrast, in Boolean logic, the truth values of variables may only be the "crisp" values 0 or 1. Fuzzy logic has been employed to handle the concept of partial truth, where the truth value may range between completely true and completely false. Furthermore, when linguistic variables are used, these degrees may be managed by specific (membership) functions.

<h3>Problem Statement</h3>
Intelligent control systems are dramatically changing domestic technology. The so-called smart homes are environments where technological tools provide convenience and comfort to residents and contribute to the reduction of energy consumption. The term smart is used due to high communication capability between devices and the use of algorithms that analyze the profile of each resident in order to optimize the use of resources and provide custom routines. 
Existing home automation devices have the following limitations:
<ul>
<li>Context-insensitive i.e they are not application-specific Ex:- Lighting lights for a party.</li>
<li>Unable to adjust the control parameters dynamically in accordance with the varying surrounding environment.</li>
<li>No adjustment of power consumption with change in environmental conditions.</li>
<li>The scale of adjustment is fixed, no scope for adjusting light intensity using expressions like “little large”,”little low” using linguistic expressions.</li>
</ul>

The first two limitations can be solved using Machine Learning and Artificial neural networks. But given the dynamics of environment we need to take large no of inputs in order to train our model which will make it infeasible.. 

<h4>Proposed Solution</h4>
We will try to solve the above limitations using fuzzy logic in our controller for home automation system to make it more adaptive, case sensitive instead of crisp scaling and frequent tunings as in conventional systems. The design of such a controller will also be simplified using fuzzy logic which gives us an added advantage.

![](https://github.com/kukr/Fuzzy-Logic-based-Light-Intensity-Controller/blob/master/assets/fuzzy-logic-solution.png)

<h4>Fuzzy logic based Home automation :-</h4>
In our implementation we will be controlling the three most basic devices which are lights,fan and heater. 
<ol>
<li>Automatic Light control using fuzzy logic.
We shall use a dimmer circuit in order to control the intensity of light. 
The dimmer circuit would recieve control from a fuzzy based controller. A fuzzy logic controller is nothing but a set of If-then rules which makes use of membership functions in order to convert these linguistic variables into analog outputs.
We shall use light sensors which shall capture the intensity of light. 
This analog input will be given to the fuzzy controller by fuzzifying the input. The Fuzzy inference system shall analyze the input linguistic variables and convert them into output linguistic variables using the If-then rule base. Finally the defuzzification process shall convert the linguistic variable into analog output.
</li>
<li>
Automatic Fan control using fuzzy logic.
   The system of actions that shall take place will remain same except here we will be using temperature sensor in order to give analog input to our fuzzy controller.

</li>
</ol> 
<h4>Final expected outcome of work</h4>

Working prototype of fuzzy logic based home automation device with following features:

*	Controlling operation of essential electric home appliances (light bulb, fan etc.)
*	Efficient software based user interface for interactive control
*	Wireless control of appliances
*	Adaptive to environment conditions using sensors
*	Retuning is not required if the system parameters change with time 
