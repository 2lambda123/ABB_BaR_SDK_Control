# Control of the ABB robot through B&R Automation PLC - ABB's PC Software Development Kit (PC SDK)

## Requirements:

**Software:**
```bash
ABB RobotStudio, B&R Automation Studio
```
ABB RS: https://new.abb.com/products/robotics/robotstudio/downloads

ABB Developer Centre: https://developercenter.robotstudio.com

B&R Automation: https://www.br-automation.com/en/downloads/#categories=Software-1344987434933

## Project Description:

The project is focused on a simple demonstration of client / server communication via OPC UA, which is implemented in C# Console App. (Server - B&R Automation PLC, Client - C# Console App). The console application communicates with the ABB robot via the PC Software Development Kit (PC SDK) from ABB. The application uses performance optimization using multi-threaded programming.

**Notes:**

ABB's PC Software Development Kit (PC SDK) is a software tool, which enables programmers to develop customized operator interfaces for the robot controller.

**MappView (HMI):**
```bash
Simulation Address
PLC_ADDRESS = localhost or 127.0.0.1

http://PLC_ADDRESS:81/index.html?visuId=abb_move
```

The project was realized at Institute of Automation and Computer Science, Brno University of Technology, Faculty of Mechanical Engineering (NETME Centre - Cybernetics and Robotics Division).

**Appendix:**

Example of a simple data processing application (OPC UA):

[OPC UA B&R Automation - Data Processing](https://github.com/rparak/OPCUA_Simple)

Example of a simple data processing application (Robot Web Services):

[ABB Robot - Data Processing](https://github.com/rparak/ABB_Robot_data_processing/)

<p align="center">
  <img src="https://github.com/rparak/ABB_BaR_SDK_Control/blob/main/images/sdk_diagram.png" width="800" height="450">
</p>


## Project Hierarchy:

**Repositary [/ABB_BaR_SDK_Control/]:**

```bash
/ACOPOSTrak_OPCUA_Unity_App/ -> C# Application
[ Data Processing              ] /Assets/Script/ACOPOSTrak_Control/
[ Object / Light Control, etc. ] /Assets/Script/Service/
[ Individual objects (.blend)  ] /Assets/Object/Blender/
[ Scene of the Application     ] /Assets/Scenes/

/acoposTrak_simple_control/ -> Automatio Studio B&R Project
[ Main Program (control of the main state machine)                  ] /Logical/Technology/tCTRL_m/Main.c
[ Header File (auxiliary functions, declaration of variables, etc.) ] /Logical/Technology/tCTRL_m/Main.h
[ MappView Visualization                                            ] /Logical/mappView/
[ ACOPOStrak Configuration (Sectors, Shuttles, etc.)                ] /Physical/Config1/X20CP3687X/mappMotion/TrakOval/
```

## Application:

## ABB RobotStudio:

<p align="center">
  <img src="https://github.com/rparak/ABB_BaR_SDK_Control/blob/main/images/abb_app.PNG" width="800" height="450">
</p>

## HMI (Human-Machine Interface) - MappView:

<p align="center">
  <img src="https://github.com/rparak/ABB_BaR_SDK_Control/blob/main/images/mv_1.png" width="800" height="450">
  <img src="https://github.com/rparak/ABB_BaR_SDK_Control/blob/main/images/mv_2.png" width="800" height="450">
</p>

## Result:

Youtube: ...

## Contact Info:
Roman.Parak@outlook.com

## License
[MIT](https://choosealicense.com/licenses/mit/)
