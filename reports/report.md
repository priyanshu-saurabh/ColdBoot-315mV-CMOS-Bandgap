
## Simulation Results and Analysis

### Cold Start and Autonomous Startup Behavior

#### Figure: `https://github.com/priyanshu-saurabh/ColdBoot-315mV-CMOS-Bandgap/blob/main/reports/Cold_boot_concept.jpeg`

The transient startup results demonstrate the autonomous cold boot capability of the proposed MOS only reference generator. During power ramp conditions, the reference voltage rises smoothly without any external startup circuitry or bias assist network.

The startup waveform confirms that weak inversion conduction naturally establishes current flow at very low supply voltages, preventing the circuit from entering a zero current metastable state. As the supply voltage increases, the PTAT and CTAT branches gradually stabilize and the output converges toward the nominal 315 mV reference level.

---

#### Figure: `Cold_boot.png`

The cold boot response under varying supply conditions shows monotonic settling of the reference voltage during both rising and falling supply transitions. The circuit maintains stable behavior without oscillation or startup failure.

This confirms reliable startup operation for battery powered and energy harvesting systems where slow and intermittent supply ramps are common.

---

#### Figure: `Ramp_Vref_Vdd.png`

The fast ramp startup waveform illustrates the transient relationship between VDD and VREF. The reference begins conducting at very low voltage levels and quickly stabilizes near 315 mV once sufficient headroom is available.

The response validates the amplifier free architecture and confirms stable startup without overshoot or metastability.

---

#### Figure: `slowramp.png`

The slow ramp transient analysis demonstrates robust startup during gradual supply increase conditions. Even under slow voltage ramps, the reference voltage tracks predictably and settles smoothly toward the nominal output level.

This behavior is important for energy harvesting applications where supply voltage often increases slowly over time.

---

### PSRR Performance

#### Figure: `psrrvsfreqedit.png`

The PSRR simulation shows strong low frequency supply rejection close to 60 dB. The response remains relatively flat across lower frequencies before gradually rolling off at higher frequencies.

This performance is achieved using a wide swing cascode current mirror structure without operational amplifiers or large compensation capacitors. The result confirms effective isolation from supply noise while maintaining compact area and low power operation.

---

### Supply Voltage Sweep Characteristics

#### Figure: `Trans_resp.png`

The DC supply sweep validates stable operation across a wide operating range. As the supply voltage increases from near zero to higher values, the reference output gradually settles and stabilizes near 315 mV.

The circuit begins self biasing at low voltages due to subthreshold conduction and reaches full regulation around the nominal operating region. The output variation across the supply range remains minimal, demonstrating good line regulation and wide supply compatibility.

---

### PTAT Characteristics

#### Figure: `ptat_ctat_temp.png`

The PTAT waveform shows a positive temperature dependence, increasing gradually as temperature rises. This behavior originates from weak inversion MOS operation where thermal voltage contributes directly to PTAT generation.

The generated PTAT component compensates the negative temperature slope of the CTAT branch to improve overall reference stability.

---

### CTAT Characteristics

#### Figure: `ptat_ctat_temp.png`

The CTAT simulation exhibits the expected negative temperature coefficient. As temperature increases, the CTAT voltage decreases gradually because of threshold voltage variation in the MOS devices.

This complementary temperature behavior is combined with the PTAT branch to minimize overall temperature drift.

---

### Temperature Stability of VREF

#### Figure: `Temp_VAR.png`

The temperature sweep of the final reference voltage confirms highly stable operation across the complete temperature range. The variation in output voltage remains extremely small from low to high temperatures.

The balanced PTAT and CTAT contributions successfully reduce the overall temperature coefficient to approximately 15 ppm per degree Celsius, validating the theoretical compensation methodology used in the design.

---

## Overall Performance Summary

The simulation results verify that the proposed reference generator achieves:

• Stable 315 mV output reference  
• Wide supply operation  
• Autonomous cold boot startup  
• Approximately 60 dB PSRR  
• Low temperature drift  
• Smooth transient response  
• MOS only implementation without BJTs or startup circuits  

These characteristics make the design suitable for ultra low power analog and mixed signal systems, sensor interfaces, and energy harvesting applications.
