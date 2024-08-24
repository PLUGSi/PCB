# PCBs

## Overview
This repository contains the PCBs of plug base and the modules that can be used with this plug base such as a programmable timer, set timer, wireless switch, and Bluetooth module. 

## Project Structure
The repository is organized as follows:

- `plug_base/`: Contains PCB files of plug base that the various modules will connect to.
- `timer_module/`: Contains PCB files of reprogrammable timer module.
- `set_timer_module/`: Contains PCB files of set timer module.
- `wireless_switch_module/`: Contains PCB files of wireless switch module.
- `bluetooth_module/`: Contains PCB files of Bluetooth module.


## Plug_Base
### Components
- **CD4041**: CMOS quad NAND Schmitt trigger inverter, used likely as an inverter or buffer.
- **Relay**: Electromagnetic switch controlled by an electrical signal to open or close contacts.
- **Resistors**: 10kΩ and 100kΩ resistors to limit current flow.
- **Capacitors**: Used to store electrical energy (value not shown).
- **Power Supply**: Provides voltage of 3V and VCC.
- **Module Connection (P2 and P3)**: Interfaces where the different modules plug into the base.


## Timer_Module
### Components
- **CD4011BE**: Quad NAND gate IC, likely used in the timer functionality.
- **Resistors (R1 and R2)**: Limit current flow (values determine current).
- **Capacitor (C1)**: Controls the timing interval by charging and discharging.
- **Pulse Input**: Trigger for the timer.
- **Output (OUT)**: Controls a relay or switching device for the outlet.
- **Status LED**: Indicates the timer state (on or off).
- **Trigger Input**: Used to reset or start the timer.


## Set_Timer_Module
### Components
- **IC1 (555 Timer)**: Functions as a voltage-controlled timer in a monostable configuration.
- **Resistors (R1 and R2)**: Work with C1 to determine timer duration.
- **Capacitor (C1)**: Sets the timer duration by controlling charge/discharge cycles.
- **Push Button (SW1)**: Trigger to initiate the timer.
- **LED1**: Visual indicator of timer status.
- **Output (OUT)**: Controls a relay or switching device for the outlet.


## Wireless_Switch_Module
### Components
- **IC1 (CD4017BE)**: CMOS IC with decade counter/divider stages, used to decode wireless signals.
- **Resistors (R1, R2, R3, R4)**: Limit current and set voltage levels.
- **Capacitor (C1)**: Filters noise on the power supply line.
- **Receiver (DI)**: Antenna or receiver circuit for the wireless signal.
- **Output (OUT)**: Controls a relay or switching device for the outlet.
- **Status LED**: Indicates the receiver module state (on or off).


## Bluetooth_Module
### Components
- **Microcontroller (U1)**: Controls the Bluetooth module and communicates with other devices.
- **Crystal (Y1)**: Provides precise oscillating signal for synchronization.
- **Resistors**: Limit current, set voltage levels, and bias transistors.
- **Capacitors**: Filter power supply, store energy, and provide stability.
- **Inductor (L1)**: Part of the matching circuit for the Bluetooth antenna.
- **Bluetooth Antenna**: Transmits and receives Bluetooth signals.
- **Status LED**: Indicates Bluetooth module state (powered on, connected, etc.).
- **Connection Pins (PBO - P5)**: Connect the Bluetooth module to the main plug base unit.

## Usage
### **Navigate to the Desired Module/PlugBase**:
  1. [`Plug Base`](./1.%20Plug%20Base)
  2. [`Reprogrammable Timer`](./2.%20Reprogrammable%20Timer)
  4. [`Set Timer`](./3.%20Set%20Timer)
  5. [`Wireless Switch`](./4.%20Wireless%20Switch)
  6. [`Bluetooth module`](./5.%20Bluetooth%20module)

### Dimensions and Pictures

<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/1937cbd2-13c9-4142-b2c2-f12614af782e" width="100%" /><br>Base</td>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/484445d3-7790-47af-830a-191ace101f9c" width="100%" /><br>Wireless Module</td>
    <td><img src="https://github.com/user-attachments/assets/10953dca-7959-471f-84c0-9ac3f928934e" width="100%" /><br>Set Timer</td>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/f03e53ba-3999-4042-910d-eb45fda7cc6d" width="100%" /><br>Reprogrammable Timer</td>
    <td><img src="https://github.com/user-attachments/assets/f49d6d88-45dd-4c1a-b65d-317c22c8f7e8" width="100%" /><br>Bluetooth</td>
  </tr>
</table>

### **Open the PCB Files**:
Use Altium PCB design software to open files.

