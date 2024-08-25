# Common-Drain-Amplifier-Design-Flow
This project covers the complete design process for a Common Drain Source Amplifier, a critical component in analog electronics.

**1. Schematic Design**

In a Common Drain (Source Follower) Amplifier using NMOS transistors, the design is configured as follows:

Circuit Configuration:

NMOS Transistor:
Source: The source of the NMOS transistor serves as the output terminal. This is where the amplified output signal is taken.
Gate: The gate is connected to the input signal. This is where the signal that you want to amplify is applied.
Drain: The drain is connected to the supply voltage (VDD), providing the necessary power for the transistor's operation.
Biasing:

VBIAS: A DC voltage source (VBIAS) is applied to the gate of the NMOS transistor to ensure it operates in the correct region of its characteristic curve. The value of VBIAS is chosen to set the appropriate operating point (DC bias point) for the transistor, ensuring it operates in its active region for proper amplification.

Connections:

Input Signal: Applied to the gate of the NMOS transistor.
Output: Taken from the source of the NMOS transistor.
Power Supply: VDD is connected to the drain of the NMOS transistor. This connection provides the power needed for the transistor to operate.
Ground: The source terminal of the NMOS transistor is typically connected to ground or a low reference voltage, ensuring that the amplifier can properly follow the input voltage.

Schematic

![Screenshot from 2024-08-20 10-32-11](https://github.com/user-attachments/assets/d7800dca-b787-446b-82bf-bf89d10ae5fd)


**2. Symbol Creation**

The symbol creation for the Common Drain (Source Follower) Amplifier involves designing a graphical representation that simplifies the integration of the amplifier into larger circuit diagrams. Here’s how you can explain this process:

Pin Configuration
In the symbol for a Common Drain Source Amplifier using NMOS transistors, the following pins are defined:

Input Pin: This pin is used to connect the input signal to the gate of the NMOS transistor.
Output Pin: This pin is where the buffered output is taken from the source of the NMOS transistor.
VDD Pin: This pin connects to the drain of the NMOS transistor and is used to supply the necessary voltage for the transistor's operation.
VSS Pin (Ground): This pin connects to the source of the NMOS transistor, which is the common terminal for the output, and often connected to ground.
VBIAS Pin: This pin is used for applying the gate bias voltage (VBIAS) to set the appropriate operating point of the NMOS transistor.
Visual Representation
The symbol should accurately reflect the NMOS transistor’s function as a voltage follower:

Design: The symbol is typically a compact, simplified version of the NMOS transistor, including:
Gate (G): Marked for the input signal.
Source (S): Marked for the output.
Drain (D): Marked for the VDD connection.
Bias: Often indicated as a separate pin or component in the symbol.
This visual representation should be clear and easily recognizable, ensuring it can be seamlessly integrated into circuit diagrams.

Symbol Creation

![Screenshot from 2024-08-20 10-31-03](https://github.com/user-attachments/assets/72c3eae8-17b2-4183-9e57-be81d969bdd8)


**3. Testbench Setup**
The Testbench Setup is crucial for simulating and verifying the performance of your Common Drain (Source Follower) Amplifier. It allows you to apply test signals and observe how the amplifier responds, ensuring it operates as expected.

Testbench Components and Configuration
Pulse Source (VPULSE):

Purpose: Provides a time-varying input signal to test the amplifier’s dynamic response.
Configuration: Set up the pulse source to deliver a square wave or pulse signal that represents the input signal.
DC Voltage Source (VDC):

Purpose: Supplies a steady DC voltage to VDD and biasing needs.
Configuration: Connect the DC voltage source to the drain (VDD) of the NMOS transistor and any other necessary nodes (e.g., gate biasing).
Connections:

Input Signal: Connect the output of the pulse source (VPULSE) to the gate of the NMOS transistor.
Power Supply: Connect the VDC to the drain (VDD) of the NMOS transistor and any other required biasing nodes.
Output Monitoring: Connect a probe or measurement tool to the source of the NMOS transistor to observe the output response.

Testbench

![Screenshot from 2024-08-20 11-09-16](https://github.com/user-attachments/assets/3a9af960-19cd-4ba3-8b21-76e6523e4a9e)
