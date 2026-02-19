# VAEs-on-LIGO-Gravitational-Waves-data

Decoding the Cosmos: An AI's Journey to Understand Gravitational Waves
LIGO

In 2015, the LIGO observatory made history by detecting the first-ever gravitational wave, a ripple in spacetime caused by two black holes merging over a billion light-years away. This discovery, which earned a Nobel Prize, opened a new window to the universe. But analyzing these faint, cosmic whispers is incredibly complex and computationally expensive.

Could a modern AI learn to do it faster?

This project explores that question using a deep learning model trained to listen to the universe and decode the secrets of black holes.

The Challenge: A Universe of Data, But Few Labels
Training an AI requires a massive amount of data with known answers (labels). While LIGO has detected ~90 events, this is a tiny dataset for deep learning. Furthermore, the "true" mass and spin of the black holes aren't known with 100% certainty—they are the results of lengthy, complex analyses.

So, how do we teach an AI?

Our Solution: A Two-Stage Learning Journey
We used a powerful technique called Transfer Learning, which mimics how a student learns: first from a textbook, then from real-world experience.

Phase 1: Learning Physics from a Perfect Textbook
We generated a large, synthetic dataset of 1000 gravitational wave signals using the same physics models (IMRPhenomD) that professional LIGO researchers use. For each signal, we knew the exact mass and spin of the black holes.

Our AI, a Variational Autoencoder (VAE), studied this perfect textbook, learning the intricate relationship between a signal's shape and its physical parameters.

Phase 2: A Real-World Internship
After mastering the theory, the AI did a short "internship" with real LIGO data. We fine-tuned the model on a small set of 5 actual gravitational wave events, teaching it to adapt its theoretical knowledge to the messy, noisy reality of the detectors.

The Final Exam: Predicting GW150914
We put our trained AI to the ultimate test: analyzing the famous GW150914 signal, the very first one ever detected.

The Results: A Stunning Success
The AI's predictions are remarkably accurate, showcasing the power of this approach.

Parameter	AI's Prediction	Actual Known Value	Error
Total Mass	~65.30 Solar Masses	~65.3 Solar Masses	< 0.1%
Effective Spin	~-0.01	~-0.06	Extremely Close
