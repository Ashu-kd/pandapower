# Following are the Power system elements considered in the model 
* Bus : 3
* Transmission line : 3
* Generator (PV) : 01
# Creation of External grid In pandapower, an External Grid (ext_grid) represents the connection of a power network to an external power source or a larger power system, typically serving as a slack or reference bus for load flow calculations. It is used to define the voltage and phase angle of a specific bus within the network and provides or absorbs active and reactive power as needed to balance the system.

Key Characteristics of ext_grid in pandapower:
* Voltage Control: Specifies a fixed voltage magnitude (in per-unit) and optionally a phase angle (in degrees) at the connected bus.

* Slack Bus Functionality: Acts as a reference point for the network, ensuring that active power mismatches are balanced during power flow calculations.

* Active and Reactive Power Supply: Provides or absorbs the necessary power to maintain the specified voltage level.

Connection to Buses: The external grid must be connected to a bus using the pp.create_ext_grid() function.             Generator EXTgrid (PV) : 01
# In pandapower, a load represents a consumer of electrical power within the network. It is modeled as a constant power load with a specified active power (𝑃) and reactive power (Q) demand. Loads are connected to buses and are essential for performing power flow calculations, as they define the power consumption at specific points in the network.

Creating a Load in pandapower:
* To create a load, the function pp.create_load() is used, which requires the following parameters:

* net: The pandapower network object.

* bus: The bus index to which the load is connected.

* p_mw: Active power consumption in megawatts (MW).

* q_mvar: Reactive power consumption in megavars (MVAr).

* name (optional): A custom name for the load.                                                                              * * Load (PQ) : 01
