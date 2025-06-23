# 🧠🔐 Image Encryption using Neural Cryptography

A lightweight and secure image encryption framework using Tree Parity Machines (TPMs), classical cryptographic techniques, and chaos theory for post-quantum-safe data protection. This layered encryption pipeline ensures high confidentiality, key sensitivity, and statistical robustness without the need for key transmission.

---

## 📌 Overview

With the rise of sensitive digital imaging in healthcare, surveillance, and cloud systems, this project addresses the growing need for secure image communication. Unlike traditional methods, this system uses neural synchronization via TPMs to derive symmetric keys without sharing them, making eavesdropping infeasible.

---

## 🔧 Features

- 🔑 **No Key Exchange Needed:** Secure key generation through TPM synchronization
- 🔁 **Fully Reversible Encryption-Decryption Pipeline**
- 🧠 **Neural Cryptography (TPMs):** Tree Parity Machines to generate secure keys
- 🧮 **Classical Ciphers:** Affine and Vigenère cipher-based transformation
- 🌪️ **Chaotic Masking:** XOR encryption using Logistic Map
- 🧪 **Tamper Detection:** Noise injection tests and error metrics for integrity validation
- 📊 **Robust Against Attacks:** High NPCR, UACI, and entropy values

---

## 📷 Workflow


---

## 🧠 Neural Key Generation (TPM)

- **Tree Parity Machine Parameters**:
  - K = 4 (hidden neurons)
  - N = 5 (inputs per neuron)
  - L = 5 (weight range)
- **Learning Rule:** Hebbian
- **Hashing:** SHA-256 or SHA-512 on the synchronized weight vector

---

## 🔐 Encryption Pipeline

1. **Fisher-Yates Shuffle:** Seeded by TPM key
2. **Zigzag Scan:** Converts 2D pixels into 1D
3. **Affine Cipher:** Linear transformation `E(x) = (a*x + b) mod 256`
4. **Vigenère Cipher:** Keyed XOR substitution
5. **Chaotic Masking:** Logistic map-based keystream for final XOR

---

## 🔁 Decryption Pipeline

- Inverse XOR (Chaotic)
- Inverse Vigenère and Affine
- Reverse Zigzag
- Inverse Fisher-Yates Shuffle

---

## 🧪 Evaluation Metrics

| Metric      | Description |
|-------------|-------------|
| **Entropy** | Target ≈ 7.99 (ideal randomness) |
| **NPCR**    | ~99.61% change rate |
| **UACI**    | 30–39% (strong diffusion) |
| **PSNR**    | 41–43 dB (high visual quality) |
| **MSE/MAE** | Low error values (good reconstruction) |
| **Correlation** | Destroyed in cipher, restored in decryption |

---

## 📊 Sample Results

- **Encrypted images:** Completely structureless
- **Decrypted images:** Perfect visual and statistical reconstruction
- **Key Sensitivity:** One-bit mismatch → full failure (PSNR ≈ 7.5 dB)

---

## 🔐 Key Space Analysis

- **TPM Key Space:** ≈ 2³⁴⁶
- **Chaotic Map:** 2²⁵⁶
- **Hash Contribution:** 2²⁵⁶ (e.g., BLAKE2b)
- **Total:** ~2⁸⁵⁸ ≈ 10²⁵⁸ (unfeasible for brute-force)

---

## 📂 Deployment Potential

- Edge IoT cameras
- Medical image security
- Cloud-secure archives
- Low-power real-time devices

---

## 👨‍💻 Authors

- **Mayank Harsh** - 2206055  
- **Divyanshi Dixita** - 2206264  
- **Abdul Subhan** - 2206270  
> Under the guidance of **Dr. Kakali Chatterjee**, Dept. of CSE, NIT Patna

---

## 📚 References

- [Autoencoder-based Image Encryption (Wang & Lo, 2024)]  
- [Chaos + Vigenère Hybrid Crypto (Ihsan & Doan, 2024)]  
- [DNA-Based IoT Encryption (Singh et al., 2022)]  
- [COVID Chest X-ray Dataset](https://github.com/ieee8023/covid-chestxray-dataset)

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.
