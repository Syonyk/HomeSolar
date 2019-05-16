# Syonyk's Home Solar Project

This is a repository for my home solar project files, in a (possibly futile) attempt to crowdsource the NEC compliance of them.  It's an iterative process, and there's no promise that what works for me will work for you.

However, the project details are unlikely to be similar to anything else you've run across, so documenting them in a public manner may be useful.

# System Design Concepts
My system is an attempt at a flexible, post-net-metering capable system.  I expect 1:1 kWh based net metering to go away (at least from my utility) inside 5 years, and I'm not certain they'll grandfather things in.  If they do, it won't be for long.  Therefore, I'm trying to build for that (unknown) future.  I also value standby power, and grid down running - which this system will get me.

Cost is in the $30k-$40k range, though the details depend on where you can source your hardware.  That price assumes you do all the work yourself, and can obtain panels at a good price locally.

The system is built to meet NEC 2017.

To avoid the per-panel rapid shutdown requirements, I am making use of the exception in 690.12, and have all the power electronics (and batteries) in a standalone shed, dedicated to solar power use.

# Panel Specifications
The panels are ITEK 295SE panels.

* Maximum Power - P<sub>MAX</sub>: 295W
* Maximum Power Voltage - V<sub>MPP</sub>: 32.8V
* Maximum Power Current - I<sub>MPP</sub>: 8.9A
* Open Circuit Voltage - V<sub>OC</sub>: 39.7V
* Short Circuit Current - I<sub>SC</sub>: 9.6A
* Temperature Coefficient of P<sub>MPP</sub>: -0.39%/C
* Temperature Coefficient of V<sub>OC</sub>: -0.29%/C
* Temperature Coefficient of I<sub>SC</sub>: +0.04%/C
* Temperature Coefficient of V<sub>MPP</sub>: -0.38%/C

Strings of 6 are used with a 300V charge controller.

Minimum expected winter design temperature is -13F/-25C.  This leads to a winter open circuit voltage of (39.7V * (1 + (0.29% * 50)) = 45.45V, or a string voltage of 272V.  This is comfortably under the 300V rating of the charge controllers.
