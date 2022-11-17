# RTT-based Wi-Fi Fingerprinting Online Radio Map Construction

## Efficient online generation of fingerprinting radio maps for indoor spaces

**Abstract**

The demand for indoor location services has exploded due to the wide range of applications they have to offer. For this purpose, classic positioning technologies (GPS among others) are not able to provide an effective response due to the low level of coverage they achieve. There are commercial solutions based on the use of Wi-Fi technology to offer this service, as it is widely deployed and accessible from practically any mobile device on the market, thus reducing the costs associated with its implementation. This work has analysed ¿fingerprinting¿, one of the positioning techniques that promises to provide the best results indoors. Its main limitation lies in the need to perform a manual mapping of the site prior to deployment. In order to have up-to-date information on the environment, mapping must be repeated frequently in these spaces due to their changing nature. The time and resource cost of such a procedure hampers the large-scale deployment of this technique. It is therefore proposed to use a Gaussian prediction model, which minimises the impact of the survey by scanning only certain points of the scenario and making a prediction of the remaining map. The main objective of the study was to determine the degree of similarity between the map generated by the algorithm and that resulting from a full manual scan. This partial scan is based on a set of time measurements over the location area, using strategically distributed Wi-Fi access points. The stability of this type of measurement is expected to reduce the update interval compared to other works in the field. Altogether, the current study proposes an efficient and innovative approach to the classical fingerprinting known to date.

**Code Description**

The purpose of the project is to implement a Gaussian Process Regressor to generate complete fingerprinting maps from a subset of RTT measurements in a predefined scenario. The Machine Learning algorithm must be trained with the set of observations and be able to generate the fingerprints on the rest of the radio map with the highest possible fidelity. The different project directories study different geometries of the scenario access points and the possibility of averaging the GPR input samples to improve the quality of the generated maps.

## Stack

Developed with jupyter Notebook technology

### Code directories

**data/dataset_sala_actos_pixel.csv** Training/Validation RTT Distance observations

**src/psfm-gpr-generation.ipynb** Generation of fingerprinting radio maps using Gaussian Process Regressor

**src/psfm-gpr-analysis-geometry.ipynb** Analysis of the impact of geometry on the quality of the generated fingerprinting maps.

**src/psfm-gpr-analysis-sample-averaging.ipynb** Analysis of the impact of the input sample averaging on the quality of the fingerprinting maps generated.

**src/layouts/*/*.ipynb** Some examples of AP layouts






