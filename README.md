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

Setting up the testbench is a critical step in verifying the performance of the amplifier. The testbench configuration includes pulse sources to simulate input signals, DC voltage sources for biasing, and measurement tools to observe the amplifier's output. The testbench schematic provided demonstrates how to connect these components to apply signals and measure the amplifier’s response effectively.

Testbench

![Screenshot from 2024-08-20 11-09-16](https://github.com/user-attachments/assets/3a9af960-19cd-4ba3-8b21-76e6523e4a9e)

**4.Simulation**

Simulation is a crucial phase in validating the performance of the Common Drain (Source Follower) Amplifier. Using Cadence Virtuoso, we perform a series of simulations to ensure that the amplifier operates according to the design specifications and performs reliably under various conditions.

1. Transient Analysis: The initial step involves transient analysis, which examines how the amplifier responds to time-varying input signals. This analysis is essential for verifying that the amplifier acts as a buffer, meaning that it provides an output that closely follows the input signal. For example, if a logical 1 (high voltage) is applied to the input, the output should also be 1, and similarly, if a logical 0 (low voltage) is applied, the output should be 0. This characteristic confirms that the amplifier is effectively buffering the signal without introducing significant distortion or delay.


![Screenshot from 2024-08-20 11-23-08](https://github.com/user-attachments/assets/6ac37079-1e35-4a4b-acc4-9cf4982fe3f5)



2. DC Response 

The DC response of a Common Drain (Source Follower) Amplifier shows that the output voltage remains constant until the input voltage reaches. Once the input voltage exceeds this threshold, the output voltage begins to closely follow the input voltage.

![Screenshot from 2024-08-20 11-22-49](https://github.com/user-attachments/assets/1653add8-7b34-44c7-b395-186769b75de9)



3. AC Analysis: Following transient analysis, i conduct an AC analysis to evaluate the frequency response of the amplifier.


![Screenshot from 2024-08-20 11-22-34](https://github.com/user-attachments/assets/f9ae92e6-c332-4cb6-b74e-104b605da1b0)



Final Simulation Result

![Screenshot from 2024-08-20 11-21-34](https://github.com/user-attachments/assets/987c3e80-75c1-4278-9408-542f68982bd2)

