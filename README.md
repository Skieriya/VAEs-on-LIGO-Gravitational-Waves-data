# VAEs-on-LIGO-Gravitational-Waves-data

We used Transfer Learning, which mimics how a student learns: first from a textbook, then from real-world experience.

# Phase 1:
We generated a large, synthetic dataset of 1000 gravitational wave signals using the same physics models (IMRPhenomD) that professional LIGO researchers use. For each signal, we knew the exact mass and spin of the black holes.

My Variational Autoencoder (VAE), studied this perfect textbook, learning the intricate relationship between a signal's shape and its physical parameters.

# Phase 2: 
After mastering the theory, the AI did a short "internship" with real LIGO data. We fine-tuned the model on a small set of 5 actual gravitational wave events, teaching it to adapt its theoretical knowledge to the messy, noisy reality of the detectors.

The Final Exam: Predicting GW150914
We put our trained AI to the ultimate test: analyzing the famous GW150914 signal, the very first one ever detected.

# The Results:
The AI's predictions are remarkably accurate, showcasing the power of this approach.

Parameter	AI's Prediction	Actual Known Value	Error
Total Mass	~65.30 Solar Masses	~65.3 Solar Masses	< 0.1%
Effective Spin	~-0.01	~-0.06	Extremely Close
