Following are the Power system elements considered in the model 
Bus : 3
Transmission line : 3
Generator (PV) : 01
# Creation of External grid In pandapower, an External Grid (ext_grid) represents the connection of a power network to an external power source or a larger power system, typically serving as a slack or reference bus for load flow calculations. It is used to define the voltage and phase angle of a specific bus within the network and provides or absorbs active and reactive power as needed to balance the system.

Key Characteristics of ext_grid in pandapower:
Voltage Control: Specifies a fixed voltage magnitude (in per-unit) and optionally a phase angle (in degrees) at the connected bus.

Slack Bus Functionality: Acts as a reference point for the network, ensuring that active power mismatches are balanced during power flow calculations.

Active and Reactive Power Supply: Provides or absorbs the necessary power to maintain the specified voltage level.

Connection to Buses: The external grid must be connected to a bus using the pp.create_ext_grid() function.             Generator EXTgrid (PV) : 01
Load (PQ) : 01
