# kamakaniokala
NASA DSCVR mission Space Apps Challenge 2022 submission by team Hui o ka la

The challenge is to improve the quality of predictions for the DSCVR spacecraft's Faraday Cup (FC) instrument using
FC data from the WIND spacecraft. Both DSCVR and WIND orbit the Earth Sun L1 Lagrange point in space so the data
if the FC instruments on these two spacecraft can be correlated.

Our approach is to use deep learning to train:
1. anomaly detector
1. proton velocity vector predictor

and combine these into a pipeline to make filter DSCVR magnetic field data and use "good" data to make ion velocity predictions.

Our stretch goal is to use transfer learning to adapt the WIND trained ion predictor to a carefully curated DSCVR data set that includes ion predictions for DSCVR.

We include 8 Jupyter notebooks:
1. explore NASA's WIND and DSCVR challenge data
2. train an anomaly detector on WIND data
3. train an ion predictor on WIND data
4. make predictions on WIND held out test set data 
5. make predictions using DSCVR data and compare with published DSCVR proton velocity vector estimates
6. produce a curated set of high quality DSCVR proton velocity vector estimates
7. use transfer learning to adapt WIND predictor to a DSCVR predictor
8. make predictions using DSCVR data and compare with published DSCVR proton velocity vector estimates
