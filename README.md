# TIBCO LABS Project AIR

**Problem Statement**: Manual labor and monitoring on water quality affected the mortality of the fishes.

**Description of Proposed Idea**: A water quality monitoring & optimization solution, based on autonomous drones, for predictive maintenance scheduling, to avoid unnecessary repair costs and production loss, in aquatic farming.

**Business Impact and Value**: Temperature is an important water quality parameter. It can affect fish and shrimp metabolism, feeding rates and the degree of ammonia toxicity. Temperature also has a direct impact on biota respiration (O2 consumption) rates and influences the solubility of O2 (warmer water holds less O2 than cooler water). With the data collected and analyzed, we will have the actionable maintenance schedules, that are optimal for a set of equipment and workforce. At the end of the day, we can eliminate human errors, while making sure, the best water quality all the time, for better production.

**High-level Approach**: Our PoC was built purely based on temperature sensor only. Later we can add more sensors, like electrical conductivity (EC), dissolved oxygen (DO), pH, salinity, carbon dioxide, ammonia, nitrite, hardness, turbidity and biochemical oxygen demand (BOD) of water.

temperature -> RPi -> mqtt -> Project AIR -> Visualization

**Differentiating Features**: The sensors will be attached at an autonomous drone, for water quality monitoring, in multiple fish ponds. The drones assignment & scheduling, will generate the time windows dynamically, according to the battery limitation, flight trajectory, temperature, waypoints order, distance between waypoints, … etc. 


**Raspberry Pi Zero 2**

![Raspberry Pi & Temperature sensor](https://i.imgur.com/9uMZ8OB.jpeg)

**DS18B20 Temperature Sensor (Waterproof)**

![DS18B20 Temperature Sensor](https://i.imgur.com/9ml8Co1.jpeg)
![DS18B20 Temperature Sensor](https://i.imgur.com/YAEm3hK.jpeg)
![DS18B20 Temperature Sensor](https://i.imgur.com/6Gs2Jjw.jpeg)


## Getting started

1. Install docker
2. get TIBCO LABS Project AIR latest Release https://github.com/TIBCOSoftware/labs-air/releases/latest 
extract
3. ./install.sh 
4. After all the processes are done you see the following 3 docker compose groups in your docker dashboard
5. Now you can access project air UI by typing localhost:8081 in your browser locally.

## Restart

1. open docker
2. play airbackend and basicdemo containers

## Reference
 
1. https://tibcosoftware.github.io/labs-air/docs/tutorials/  
2. https://tibcosoftware.github.io/flogo/labs/raspberry-iot/ 
3. https://thenewstack.io/tutorial-building-an-iot-app-with-flogo-and-raspberry-pi/
4. https://github.com/ecarlier-tibco/flogo/tree/master/application/pitemp 


