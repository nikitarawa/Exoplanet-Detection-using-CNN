**Introduction**
This project focuses on automating the detection of exoplanets using light curve data from NASA’s Kepler mission. By analyzing subtle dips in a star’s brightness, we aim to identify potential exoplanet transits using a Convolutional Neural Network (CNN). The end-to-end pipeline involves preprocessing raw CSV data, converting brightness values into model-ready tensors, building a 1D CNN in PyTorch, and evaluating its performance on test data. This approach showcases how AI can accelerate astronomical discovery by efficiently analyzing large volumes of space data

**What are Exoplantes?**
Exoplanets are the planets that orbit stars outside our solar system. 
Just like Earth orbits the Sun, exoplanets orbit other stars in the galaxy. Some are rocky like Earth, others are gas giants like Jupiter. Scientists study exoplanets to learn if there might be life beyond Earth or if some planets could be habitable!

**What is Keplers Data?**
Kepler's data comes from NASA's Kepler Space Telescope, which was launched to find exoplanets (planets outside our solar system) on March 7th 2009.
Kepler watched thousands of stars and looked for tiny dips in their brightness.
If a planet passed in front of a star (like a mini eclipse), the star's light would dim a little - which is called a transit.

**What does Keplers Data shows?**
	• How bright each star is over time (called a light curve).
	• When the brightness dips — which can mean a planet passed in front
	• By studying these dips, we can figure out If a planet is there, How big it is, How far it is from its star, How long it takes to orbit that particular Star.


**Key components include:**
	•	Dataset: Kepler-labelled time-series data from Kaggle
	•	Methods: 1D CNN trained in PyTorch for binary classification (transit vs no transit)
	•	Performance: Achieved ~99.12% accuracy and 99.56% F1-score on test data
	•	Data Processing: Noise reduction with Savitzky–Golay filter, normalisation, and visual validation of transit curves
	•	Goal: Automate exoplanet detection and improve the scalability of astronomical data analysis using deep learning

Future improvements involve addressing class imbalance, testing with TESS data, and implementing explainable AI techniques to interpret model predictions.


