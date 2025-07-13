# VLSI-TASK4-DIGITAL-FILTER

COMPANY: CODTECH IT SOLUTIONS

NAME: SYED TAUSEEF ASHRAF

INTERN ID: COMPANY: CT06DF1544

DOMAIN: VLSI

DURATION: 6 WEEKS

MENTOR: NEELA SANTOSH

*In task 4, a digital splash filter (finite impulse response) has been designed and simulated using Verilog HDL. The purpose of this task was to create a functional digital filter that performs a weighted sum of current and passed input samples using fixed coefficients. FIR filters are commonly used in digital signal processing to soften, noise reduction and signal improvement. Implementation has focused on demonstrating the main functionality of a FIR filter by simulating and wave form verification.

The filter was built using a four-tax design, which means it uses four coefficients and four delayed versions of the input signal. The filter module defines four coefficient records, labeled B0, B1, B2 and B3, which were initialized during the redefinition for specific fixed point values. Together with these coefficients, a four -record delay line was used to store the latest input samples. This structure ensures that at each clock cycle, the filter has access to the current input and three previous samples required for the calculation.

The behavior of the filter is governed by three sequential blocks. The first block deals with coefficient boot during redefinition. The second block manages the change of input samples through the delay line in all positive edges of the clock. The third block performs the calculation of the core filter by multiplying each delayed input with its respective coefficient and adding the results to form the final output. The calculated result is stored in a 32 -bit signed record and assigned to the module outlet.

To check the design, a separate test module was created. This testbench generated a regular watch signal and controlled the redefinition sequence. After the redefinition was awakened, the input values were applied at fixed time intervals to simulate a signal that enters the filter. Specifically, values such as 1000, 2000, 3000, 4000 and 5000 were supplied sequentially to observe how the filter responds as the delay line fills and the output accumulates. This allowed a step -by -step examination of filter behavior.

The simulation and wave form analysis was performed using the EDA playground platform. The forms of exit wave were observed through the Epwave, which provided a visual representation of signal changes over time. Wave shapes showed the change in input values in the delay line and the resulting output changes based on the current and past samples. The signs of restarting, clock, input and exit were all captured correctly, and the filter demonstrated the expected behavior, as defined by the FIR filter equation.

The simulation results confirmed that the filter operated correctly and the output reflected the effect of each input sample weighted by the corresponding coefficients. The waveform indicated that the values built over time, illustrating how the filter integrates several samples to form the output. This validated that the FIR filter design was working as intended.
<img width="1915" height="591" alt="T4" src="https://github.com/user-attachments/assets/2ea69dd5-be6a-4fcf-a082-809d201e85c1" />
