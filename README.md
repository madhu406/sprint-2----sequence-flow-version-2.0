# sprint-2----sequence-flow-version-2.0

# in this sprint 2 there is a updation of sprint 1 
# the following sequence diagram shows the relationship between the classes 


In the second sprint, the low level architecture for the
system is designed. 
It includes the following classes. 
• HomeOwner: Represents the homeowner.
• SmartGeyser: Represents the geyser system.
• EnvironmentSensor: Represents the environment sensor to detect season,
temprature.
• WaterHeater: Represents the water heater.

#Sequence Diagram: Calculate Heating Temperature of Water
------------------------------------------------------------------
[Homeowner] -> [Smart Home System]: Gets out of bed
[Smart Home System] -> [Bathroom Geyser]: activateGeyser()
[Bathroom Geyser] -> [Temperature Sensor]: Get current temperature
[Temperature Sensor] -> [Bathroom Geyser]: Current temperature
[Bathroom Geyser]->[HeatingSystem]: Calculate required temperature
[Heating System] --> [Bathroom Geyser]: Required temperature
[Bathroom Geyser] --> [Smart Home System]: Heating temperature
[Smart Home System] --> [Homeowner]: Geyser activated
 
 # in this sequence diagram the Homeowner is directly connected to Smart Home System which provide the information about the homeowner
 # similarly for the Smart Home System is connected with Bathroom Geyser which is used to activate the Geyser
 
