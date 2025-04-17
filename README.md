This repository explores Objectosphere-Tuned models for improving out-of-distribution (OOD) detection, building upon baseline and energy-based (EOS) approaches. The focus is on enhancing separation between known and unknown samples in both softmax confidence (MSP) and feature magnitude space.

🔍 Overview
We analyze and compare three methods:

Baseline Model

Energy-based OOD Scoring (EOS)

Objecto-Tuned Model (λ=0.5, ξ=30.0)

The goal is to enforce a margin in the feature space that helps distinguish unknown samples during inference.

📊 Key Observations
Max Softmax Probability (MSP)
Known samples cluster near MSP = 1.

Unknown samples show a clearer separation as we move from baseline → EOS → Objecto-Tuned.

Feature Magnitude
The Objectosphere-tuned model enforces a margin ξ=30.0.

Known samples lie predominantly above ξ, while unknowns fall below, confirming improved feature-space separation.
