# Lab-0
ME 405 

Our program runs a step response test, located on the microcontroller.
It then sends to data to our PC via serial port. 

![ME405_Lab0_Voltage_Time_Graph](https://github.com/alialauren1/Lab-0/assets/157066441/8ecfbebd-9b0b-4df4-8476-36fc024288a7)

On the micropython board a program has been created to set pin C0. A circuit connected to C0 consisting of two resistors and a capacitor which then then outputted to the ADC pin on then board. The program takes voltage measurements every 20 ms. The timing of each measurement is controlled using an ISR on the board. The captured data is then tabulated in a CSV formatting and is sent to the connected PC via the serial port. On our the PC a program that creates a GUI and reads the CSV data that has been sent through the serial port. The voltage data is then plotted against time. The code also calculates the theoretical response of the circuit using V(t) = V_max*(1-exp(-t/(RC)).

Our results are slightly offset from the theoretical value. We 
