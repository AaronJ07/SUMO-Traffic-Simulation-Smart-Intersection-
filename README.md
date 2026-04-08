# SUMO-Traffic-Simulation-Smart-Intersection-
This project simulates a traffic light-controlled intersection using Simulation of Urban MObility (SUMO). It demonstrates basic traffic flow, routing and signal control at a four-way junction.

⚙️ Requirements
Install SUMO:
👉 https://www.eclipse.org/sumo/
Make sure SUMO is added to your system PATH bu using this command in CMD: sumo --version

*The road network is automatically generated using Simulation of Urban MObility (netconvert tool).

🚀 How to Run the Simulation
1. Navigate to project folder: cd your-project-folder

2. Run with GUI: sumo-gui -c cross.sumocfg
   This will open the graphical simulation where you can:
   See vehicle movement
   Observe traffic light behavior
   Analyze congestion

OR

3. Run without GUI (CLI mode): sumo -c cross.sumocfg

🧠 Simulation Overview
Network
A 4-way intersection (North, South, East, West)
Defined using:
Nodes → cross.nod.xml
Edges → cross.edg.xml

🚗 Traffic Flow

Defined in: cross.rou.xml

Includes:
1. Cars and trucks
2. Multiple routes:
    North → South
    West → East
    South → East (turning)

🚦 Traffic Light Logic

Defined inside: cross.net.xml

IMPORTANT (You may use this test example to test wether your SUMO is working well or not)
🧪 Test Example
A simple test network is also included:

hello.sumocfg

Run it with: sumo-gui -c hello.sumocfg

This is useful for:
1. Beginners
2. Debugging configuration issues

📈 Future Improvements:
1. Adaptive traffic light using AI
2. Emergency vehicle priority (green wave)
3. Integration with reinforcement learning
4. Real-time traffic optimization

👨‍💻 Author
TENG

📜 License
This project is open-source and free to use for educational purposes.

💡 Notes
If simulation does not run:
1. Ensure all .xml files are in the same directory
2. Check cross.sumocfg file paths
3. Validate XML syntax
