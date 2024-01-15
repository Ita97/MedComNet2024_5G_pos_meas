# 5G Positioning Raw Measurement Dataset 
This repository contains datasets of 5G positioning measurements simulated in a realistic environment using a Matlab raytracer tool.
These measurements are analyzed in a paper submitted to MedComNet 2024, which will be held on June 2024 in Nizza, France.

Each row of the datasets is composed of the following:
- Base Station (BS) coordinates (x, y, z)
- User Equipment (UE) coordinates (x, y, z)
- Raw measurements (TDOA/AOA/TOA)
- Timestamp of measurement acquisition (1-100)

For each UE position, 100 Monte-Carlo simulations are performed. The timestamp indicates in which Monte-Carlo simulation the measurement is acquired.
The first BS for each timestamp is the reference BS used to compute the TDOA; therefore, no TDOA measurement is shown for that BS.
<p align="center">
  <img src="https://github.com/Ita97/ICASSP2024_5G_pos_meas/assets/28793450/95bd75bd-5e05-445e-b456-8e47111b804e"  width="500"  /></center>
</p>
The dataset called "5x5_square" contains measurements taken in Piazza Duomo, Milan, Italy, in 25 points, where the multipath effect is at its minimum (blue square).
Instead, the "trajectory" dataset contains measurements taken in a trajectory of 28 points (red dots) with harsh conditions (i.e., BSs in non-line-of-sight and high multipath effect).
