# Proof of Everything: Verifiable Object and Event Authentication

Welcome to the **Proof of Everything** project! This repository is part of the Proof-of-Every-Thing-Eth-Oxford organization and aims to combine **cryptography**, **machine learning**, and **acoustic signatures** to create a privacy-preserving system that proves the authenticity of objects, events, and individuals—**on-chain**.

> **See our [Presentation](https://www.canva.com/design/DAGejCBzjx4/mQu49B6K0e26smrSgZlrxg/edit?utm_content=DAGejCBzjx4&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton) for an overview of the project.**

---

## Project Diagram

Below is a high-level diagram that explains how our system works:

![Project Diagram](../images/diagram.png)

---

## Quick Links

- **[Presentation](https://www.canva.com/design/DAGejCBzjx4/mQu49B6K0e26smrSgZlrxg/edit?utm_content=DAGejCBzjx4&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)**  
  An introductory walkthrough of the project’s goals, technology, and vision.

---

## Repositories in This Organization

1. **[Music Archive App](https://github.com/Proof-of-Every-Thing-Eth-Oxford/music-archive-app)**
   - A Mina zkApp that enables verifiable, privacy-preserving liveness detection by cryptographically linking audio recordings to a timestamped on-chain state.

2. **[proof_gen](https://github.com/Proof-of-Every-Thing-Eth-Oxford/proof_gen)**
   - Explores the bridge between Halo2 (EZKL) and MINA using different approaches, including zkVMs like RISC0 and SP1.

3. **[prover-of-every-thing](https://github.com/Proof-of-Every-Thing-Eth-Oxford/prover-of-every-thing)**
   - A React Native app that performs the proving of every thing, providing the interface for generating cryptographic proofs.

4. **[verifiable-echo-ml-model](https://github.com/Proof-of-Every-Thing-Eth-Oxford/verifiable-echo-ml-model)**
   - Contains experiments and scripts to build, train, and export an audio+image verification model that underpins the system’s authentication process.

---

## Problem Statement

In an era where deepfakes and digital manipulation challenge the authenticity of digital content, our project bridges the gap between physical reality and digital trust. Originally designed for human liveness verification, our system has evolved into a **Proof of Everything** mechanism that cryptographically authenticates objects, people, and events.

---

## Technical Innovation

### 3D Acoustic Fingerprinting
- **Acoustic Signatures:** We generate 3D acoustic “fingerprints” of objects using sound waves—similar to LiDAR, but privacy-preserving and lightweight.
- **Challenge Sound:** A unique sound is generated every 3 minutes using a **Mina blockchain hash** to seed the randomness, ensuring each verification is unique and time-bound.

### Echo-Based Object Authentication
1. **Sound Emission:** The device plays the challenge sound aloud.
2. **Echo Capture:** The returning echo is recorded, forming an acoustic signature of the object or environment.
3. **Multi-Modal Verification:** A compact neural network processes:
   - The original **challenge sound**
   - The captured **echo**
   - A **reference image**
   
   to verify the authenticity of the object.

> **For more details on the system workflow, refer to our [Presentation](https://www.canva.com/design/DAGejCBzjx4/mQu49B6K0e26smrSgZlrxg/edit?utm_content=DAGejCBzjx4&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton).**

### Publicly Verifiable Randomness & Zero-Knowledge Proofs
- **Randomness:** Every challenge sound is seeded with publicly verifiable randomness from the Mina blockchain, linking the verification to a specific time.
- **Privacy Preservation:** We employ Zero-Knowledge Proofs (ZKPs) using **EZKL** to prove the correct execution of our model without exposing raw sensor data or internal details.
- **On-Chain Attestation:** The generated proofs can be verified by Mina zkApps, ensuring that the process is both transparent and secure.

---

## Privacy-Preserving Architecture

- **Local Inference:** All processing occurs on the user's device, preserving privacy.
- **Efficient Model:** A custom, compact neural network processes two audio inputs and one image while keeping resource usage low.
- **Zero-Knowledge Proofs:** Utilizing EZKL, we generate proofs that verify the integrity of the local inference without exposing sensitive data.

---

## Applications & Potential Impact

1. **Digital Identity & Liveness Verification**
   - **Remote Authentication:** Proving that users are real, preventing deepfake-based fraud and ensuring sybil resistance in Web3 applications.
  
2. **Real-World Event Verification**
   - **Logistics & Deliveries:** Cryptographically verifiable proofs of package drop-offs.
   - **Infrastructure Monitoring:** Secure, sound-based authentication of physical environments in security-sensitive areas.
  
3. **Privacy-Preserving Signatures**
   - **Timestamped, On-Chain Proofs:** Providing verifiable evidence of events without exposing private information.
   - **Digital-Physical Trust:** Authenticating physical objects for supply chain management, anti-counterfeiting, and more.

---

## Next Steps

- **Recursive ZK Proofs:** Exploring nested or recursive proofs on the Mina blockchain for enhanced scalability and trust.
- **Advanced AI Models:** Expanding the model to authenticate more complex structures and environmental changes.
- **Industry Partnerships:** Collaborating with security, AI, and Web3 firms to deploy and scale our technology.

---

## Conclusion

In a world where digital content can be easily manipulated, **Proof of Everything** offers a novel way to authenticate real-world events and objects using **sound-based verification** and **zero-knowledge proofs**. Our system ensures that what is captured is both real and verifiable—all while preserving user privacy.

> **Learn more by checking out our [Presentation](https://www.canva.com/design/DAGejCBzjx4/mQu49B6K0e26smrSgZlrxg/edit?utm_content=DAGejCBzjx4&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton).**

We welcome your feedback, collaborations, and contributions as we continue to push the boundaries of digital trust and privacy.

---

Thank you for your interest in our project!
