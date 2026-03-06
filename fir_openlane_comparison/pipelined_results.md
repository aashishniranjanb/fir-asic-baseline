# ASIC Results: Pipelined FIR

**Key Takeaway for Research Day Presentation:**
Inserting pipeline registers successfully broke the critical path. The Pipelined FIR achieved full timing closure (0.0 ns WNS/TNS) at 153.8 MHz, fixing the setup violations seen in the Direct-Form baseline. The tradeoff is a 22% increase in core area (114,034 µm² vs 93,330 µm²) and a slight increase in energy per sample (63.7 pJ vs 56.3 pJ) due to the added flip-flops. 

## Extracted Metrics (from OpenLane metrics.csv)
* **Clock Period:** 6.5 ns 
* **Operating Frequency:** 153.8 MHz
* **WNS (Worst Negative Slack):** 0.0 ns 
* **TNS (Total Negative Slack):** 0.0 ns
* **Total Standard Cells:** 14,906
* **Core Area:** 114,034 µm²
* **Total Power:** ~9.80 mW
* **Energy/Sample:** ~63.7 pJ
