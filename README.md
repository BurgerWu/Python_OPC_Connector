# Python_OPC_Connector
<img src="images/OPC.png" height='120'><img src="images/PY.png" height='120'>
## Introduction
OPC (Open Platform Communication) is the interoperability standard for the secure and reliable exchange of data in the industrial automation space and in other industries(From OPC Foundation). It was first built on the demand of integrating complex vendor specific protocol(ex: Modbus, Profibus and etc) into a standard one. OPC was once called OLE (Object Linking and Embedding) for process control, and it highly depends on Microsoft’s OLE, COM(Component Object Model) and DCOM(Distributed Component Object Model) technlogy. This early development of OPC was also called OPC classic with three major division: OPC DA(Data Access), AE(Alarms and Events) and HDA(Historical Data Access).

OPC UA was released in 2008, it integrated the functionality and specifications of OPC Classic into an extensible framework (From OPC Foundation). OPC UA not only works as reliable as OPC DA does, it also eliminates the platform restriction, comes with stronger authentication and encryption mechanism. What is the most important is, it saves time on configuration because OPC UA no longer relies on COM/DCOM.

This project uses Python language as client tool to connect to OPC DA and OPC UA servers.

## Packages Used
**1. OPC DA:**
- OpenOPC-Python3X: Main package for OPC DA connection
- pywin32: Python for win32 extensions
- Pyro4: Allow application objects to talk to each other

**2. OPC UA:**
- opcua: Main package for OPC UA connection

**3. Real-Time Plotting**
- matplotlib

## Files and Directory
- OPCDA_Python.html: HTML of rendered OPCDA Python notebook
- OPCDA_Python.ipynb: OPCDA Python notebook
- OPCUA_Python.html: HTML of rendered OPCUA Python notebook
- OPCUA_Python.ipynb: OPCUA Python notebook

## Content 
In the notebook, we demonstrate the basic codes required to build connection, read/write values and explore hierachy. Also, a real-time animation that shows data acquisition from OPC server is implemented as well. If you want to know some more detail as well as hints when dealing with errors, you are welcome to visit my medium post regarding this Python OPC connector project:<a href='https://medium.com/@burgercewu/connecting-opc-servers-using-python-b774d630acb'> Connecting OPC Servers Using Python</a>

## Conclusion
In this project, we demonstrate basic functions of OpenOPC-Python3X and opcua so that users can create connections to OPC server no matter what their application is for. Real-time plotting from the repo of this project proves the reliability and feasibility of the connection with OPC server. However, the setting of OpenOPC to OPC DA server is relatively troublesome and requires much more trial and error. Based on this result, it is highly recommended that you go for OPC UA if possible since OPC UA is considered to be the standard connection specification of state-of-the-art industrial automation.
