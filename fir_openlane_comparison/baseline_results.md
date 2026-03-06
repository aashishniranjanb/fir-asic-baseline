# ASIC Baseline Results: Direct-Form FIR

**Key Takeaway for Research Day Presentation:**
We can now definitively state that the Direct-Form FIR fails to meet timing at 153.8 MHz (6.5 ns). Because it lacks pipeline registers, the critical path through the multiplier and adder tree is simply too long. This perfectly sets up the argument for why the Pipelined and Slack-Aware architectures are physically necessary to hit high frequencies.

## Extracted Metrics (from OpenLane metrics.csv & rcx_sta.max.rpt)
* **Target Clock Period:** 6.5 ns (153.8 MHz)
* **Achievable Clock Period:** 7.73 ns (129.36 MHz)
* **WNS (Worst Negative Slack):** -1.23 ns (at 6.5ns target - Setup Violations Confirmed)
* **TNS (Total Negative Slack):** -18.81 ns
* **Total Standard Cells:** 12,015
* **Core Area:** 93,330 µm²
* **Total Power:** ~7.29 mW (0.00474 W Internal + 0.00255 W Switching)
* **Energy/Sample:** ~56.3 pJ (Calculated as 7.29 mW / 129.36 MHz)
