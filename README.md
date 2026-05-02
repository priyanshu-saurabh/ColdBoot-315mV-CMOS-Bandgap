# 315 mV MOS Only Voltage Reference for Low Power Systems

This repository presents the complete development flow of a compact CMOS voltage reference designed for ultra low power and energy constrained applications. The project implements a fully MOS based reference architecture capable of generating a stable 315 mV output while operating across a wide supply range from 1 V to 5 V.

The circuit is built using PTAT and CTAT behavior generated entirely from MOS transistors operating in weak and moderate inversion. A wide swing cascode current mirror is used to improve output resistance, supply rejection, and current scaling accuracy while maintaining low voltage operation.

One of the important characteristics of this design is its natural cold boot capability. Since weak inversion conduction exists even at very low voltages, the circuit starts autonomously during both slow and fast supply ramps without requiring any external startup circuitry.

## Main Highlights

• 315 mV stable reference output  
• Wide supply operation from 1 V to 5 V  
• Fully MOS based architecture  
• Approximately 15 ppm per degree Celsius temperature coefficient  
• Around 60 dB low frequency PSRR  
• Autonomous startup capability  
• Optimized for low power mixed signal and energy harvesting systems  



This project focuses on reliable low voltage reference generation for modern analog and mixed signal integrated systems where power efficiency, startup robustness, and compact implementation are critical.
