# TIBCO LABS Project AIR

**Problem Statement**: Manual labor and monitoring on water quality affected the mortality of the fishes.

**Description of Proposed Idea**: A water quality monitoring & optimization solution, based on autonomous drones, for predictive maintenance scheduling, to avoid unnecessary repair costs and production loss, in aquatic farming.

**Business Impact and Value**: Temperature is an important water quality parameter. It can affect fish and shrimp metabolism, feeding rates and the degree of ammonia toxicity. Temperature also has a direct impact on biota respiration (O2 consumption) rates and influences the solubility of O2 (warmer water holds less O2 than cooler water). With the data collected and analyzed, we will have the actionable maintenance schedules, that are optimal for a set of equipment and workforce. At the end of the day, we can eliminate human errors, while making sure, the best water quality all the time, for better production.

**High-level Approach**: Our PoC was built purely based on temperature sensor only. Later we can add more sensors, like electrical conductivity (EC), dissolved oxygen (DO), pH, salinity, carbon dioxide, ammonia, nitrite, hardness, turbidity and biochemical oxygen demand (BOD) of water.

temperature -> RPi -> mqtt -> Project AIR -> Visualization

**Differentiating Features**: The sensors will be attached at an autonomous drone, for water quality monitoring, in multiple fish ponds. The drones assignment & scheduling, will generate the time windows dynamically, according to the battery limitation, flight trajectory, temperature, waypoints order, distance between waypoints, … etc. 