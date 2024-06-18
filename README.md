# PCBs

## Overview
This repository contains the PCBs of plug base and the modules that can be used with this plug base such as a programmable timer, set timer, wireless switch, and Bluetooth module. 

## Project Structure
The repository is organized as follows:

- `plug_base/`: Contains PCB files for the plug base that the various modules will connect to.
- `timer_module/`: Contains PCB files for a reprogrammable timer module.
- `set_timer_module/`: Contains PCB files for a set timer module.
- `wireless_switch_module/`: Contains PCB files for a wireless switch module.
- `bluetooth_module/`: Contains PCB files for a Bluetooth module.


## Plug Base
### Components
- **CD4041**: CMOS quad NAND Schmitt trigger inverter, used likely as an inverter or buffer.
- **Relay**: Electromagnetic switch controlled by an electrical signal to open or close contacts.
- **Resistors**: 10kΩ and 100kΩ resistors to limit current flow.
- **Capacitors**: Used to store electrical energy (value not shown).
- **Power Supply**: Provides voltage of 3V and VCC.
- **Module Connection (P2 and P3)**: Interfaces where the different modules plug into the base.


## Timer Module
### Components
- **CD4011BE**: Quad NAND gate IC, likely used in the timer functionality.
- **Resistors (R1 and R2)**: Limit current flow (values determine current).
- **Capacitor (C1)**: Controls the timing interval by charging and discharging.
- **Pulse Input**: Trigger for the timer.
- **Output (OUT)**: Controls a relay or switching device for the outlet.
- **Status LED**: Indicates the timer state (on or off).
- **Trigger Input**: Used to reset or start the timer.


## Set Timer Module
### Components
- **IC1 (555 Timer)**: Functions as a voltage-controlled timer in a monostable configuration.
- **Resistors (R1 and R2)**: Work with C1 to determine timer duration.
- **Capacitor (C1)**: Sets the timer duration by controlling charge/discharge cycles.
- **Push Button (SW1)**: Trigger to initiate the timer.
- **LED1**: Visual indicator of timer status.
- **Output (OUT)**: Controls a relay or switching device for the outlet.


## Wireless Switch Module
### Components
- **IC1 (CD4017BE)**: CMOS IC with decade counter/divider stages, used to decode wireless signals.
- **Resistors (R1, R2, R3, R4)**: Limit current and set voltage levels.
- **Capacitor (C1)**: Filters noise on the power supply line.
- **Receiver (DI)**: Antenna or receiver circuit for the wireless signal.
- **Output (OUT)**: Controls a relay or switching device for the outlet.
- **Status LED**: Indicates the receiver module state (on or off).


## Bluetooth Module
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
1. **Navigate to the Desired Module**:
  cd plug_base
  # or
  cd timer_module
  # or
  cd set_timer_module
  # or
  cd wireless_switch_module
  # or
  cd bluetooth_module
  
3. **Open the PCB Files**:
Use Altium PCB design software to open files.

