# PROJECT.md

## **Project Title: Post-Quantum Cryptography Simulator**
This project will demonstrate the vulnerabilities of classical cryptographic systems, such as RSA, to quantum attacks (notably Shor's algorithm). It will also explore post-quantum cryptographic schemes as alternatives, using a hands-on approach to implement and benchmark both classical and post-quantum algorithms.

---

## **1. Project Overview**

### **Purpose**
- To **implement and simulate RSA**, providing a foundational understanding of classical cryptography.
- To **demonstrate quantum attacks**, focusing on Shor's algorithm, highlighting the vulnerabilities of RSA to quantum computing.
- To **explore post-quantum cryptography (PQC)**, such as lattice-based cryptographic schemes, showcasing their resistance to quantum attacks.
- To produce an **educational toolkit** with code, documentation, and benchmarks suitable for public sharing (e.g., GitHub/LinkedIn).

### **Motivation**
As quantum computing advances, classical cryptographic systems like RSA face obsolescence. Organizations must transition to post-quantum algorithms to ensure data security. This project provides an entry-level-friendly yet comprehensive toolkit to demonstrate this critical transition.

---

## **2. Deliverables**

1. **RSA Implementation**:
   - Python-based implementation of RSA encryption, decryption, and key generation.
   - Example use cases with plaintext and ciphertext.

2. **Quantum Attack Simulation**:
   - Demonstration of Shor’s algorithm using IBM Quantum Cloud and Qiskit to factor small integers.
   - Analysis of Shor's implications on RSA's security.

3. **Post-Quantum Cryptography Demonstration**:
   - Implementation of a lattice-based cryptographic scheme (e.g., Kyber or Dilithium).
   - Benchmarking post-quantum schemes against RSA in terms of key size, encryption time, and decryption time.

4. **Educational Materials**:
   - A well-documented Jupyter Notebook to walk through RSA, Shor’s algorithm, and post-quantum cryptographic techniques.
   - Visualizations of performance benchmarks and security comparisons.

5. **GitHub Repository**:
   - All code, documentation, and resources will be packaged into a public GitHub repository with a detailed README.

---

## **3. Key Features**

1. **Hands-On RSA Implementation**:
   - Fully functional RSA implementation, from key generation to encryption/decryption.

2. **Shor’s Algorithm Integration**:
   - Simulated attacks on small RSA keys using Qiskit, demonstrating the theoretical power of quantum attacks.

3. **Post-Quantum Cryptography**:
   - Focus on NIST Round 3 finalists like Kyber for key encapsulation and Dilithium for digital signatures.

4. **Benchmarking Framework**:
   - Compare classical and post-quantum schemes in terms of:
     - Security (e.g., resistance to quantum attacks).
     - Performance (key generation time, encryption/decryption time, etc.).
     - Resource efficiency (memory and key size).

---

## **4. Project Roadmap**

### **Phase 1: Classical Cryptography Foundations**
- Implement RSA with Python.
- Test RSA implementation with small plaintext messages.
- Validate encryption/decryption correctness with unit tests.
- Deliverable: `rsa.py` and test scripts.

### **Phase 2: Quantum Threat Modeling**
- Study Shor's algorithm and its impact on RSA.
- Implement Shor's algorithm with Qiskit for small integers (e.g., 15, 21).
- Analyze the practicality of quantum attacks using current hardware.
- Deliverable: `shor_demo.ipynb` notebook.

### **Phase 3: Transition to Post-Quantum Cryptography**
- Implement a lattice-based cryptographic scheme (e.g., Kyber or Dilithium).
- Demonstrate key encapsulation and digital signatures.
- Benchmark post-quantum schemes against RSA.
- Deliverable: `pq_kem.py` and `pq_benchmark.ipynb`.

### **Phase 4: Real-World Protocol Integration**
- Simulate a TLS handshake using RSA and then substitute a post-quantum key exchange.
- Evaluate real-world performance and feasibility.
- Deliverable: `tls_simulation.py`.

### **Phase 5: Final Documentation and Deployment**
- Prepare educational materials (tutorial notebooks, visualizations, diagrams).
- Publish GitHub repository with a polished README.
- Optional: Deploy a static site or blog summarizing findings.
- Deliverable: Complete project repository with comprehensive documentation.

---

## **5. Tools and Technologies**

1. **Programming Languages**:
   - Python (for cryptographic implementations and simulations).

2. **Libraries and Frameworks**:
   - Qiskit: For quantum computing simulations and Shor’s algorithm.
   - `cryptography` and `sympy`: For classical cryptographic operations.
   - Matplotlib/Plotly: For performance visualizations.
   - pytest: For testing.

3. **Platforms**:
   - IBM Quantum Cloud: For running quantum algorithms.
   - AWS/Google Cloud: For classical cryptographic benchmarks and larger simulations.

4. **Standards and References**:
   - RSA Standard (RFC 8017).
   - NIST Post-Quantum Cryptography Standardization Documentation.

---

## **6. Learning Resources**

### **For Classical Cryptography**
- *"Introduction to Modern Cryptography"* by Katz & Lindell.
- RSA Documentation: [RFC 8017 (PKCS #1)](https://tools.ietf.org/html/rfc8017).
- Cryptopals challenges: [https://cryptopals.com/](https://cryptopals.com/).

### **For Quantum Computing**
- Qiskit Textbook: [https://qiskit.org/textbook/](https://qiskit.org/textbook/).
- *Quantum Computation and Quantum Information* by Nielsen & Chuang.

### **For Post-Quantum Cryptography**
- NIST PQC Project: [https://csrc.nist.gov/Projects/post-quantum-cryptography](https://csrc.nist.gov/Projects/post-quantum-cryptography).
- Kyber Documentation: [https://pq-crystals.org/kyber/](https://pq-crystals.org/kyber/).

---

## **7. Performance Benchmarks**

Key metrics for comparison:
1. **Key Size**:
   - RSA: Large public/private keys (~2048 bits).
   - Post-Quantum (Kyber): Smaller key sizes (~1000-3000 bytes, depending on parameters).

2. **Encryption/Decryption Time**:
   - Measure average encryption and decryption times for both RSA and Kyber.

3. **Security**:
   - Highlight vulnerabilities of RSA to quantum attacks.
   - Explain why lattice-based cryptography resists quantum threats.

---

## **8. Success Criteria**

The project will be considered successful if:
1. A complete RSA implementation is provided, with functional encryption, decryption, and key generation.
2. Shor’s algorithm is successfully demonstrated on small integers using Qiskit.
3. A post-quantum cryptographic scheme is implemented and benchmarked.
4. All code, documentation, and educational materials are packaged in a polished GitHub repository.

---

## **9. Contribution and Future Work**

### **Opportunities for Extension**
- Expand the toolkit to include additional post-quantum algorithms (e.g., hash-based or code-based cryptography).
- Explore hybrid quantum-classical workflows for cryptographic operations.
- Investigate how noise and error mitigation affect Shor's algorithm's success rate.

### **Community Contribution**
Feel free to fork the repository and suggest improvements or additional features. Contributions to this project will help raise awareness about the importance of transitioning to post-quantum cryptography.

---

## **10. Contact**

For questions or feedback, please reach out via GitHub issues or email. Contributions, bug reports, and suggestions are welcome.
