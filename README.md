# Hi, I’m Adit Sharma

I am an undergraduate Computer Science student at the University of Illinois Chicago (Class of ’28, Software Engineering). My academic and project work sits at the intersection of **systems programming, security, and machine learning**, where I enjoy building reliable, test-driven solutions. I approach problems by breaking them into measurable parts, designing scalable, fault-tolerant solutions to ensure reliability, and documenting my decisions clearly to ensure transparency and accountability.

In the last year, I developed a **container vulnerability scanner** that reduced CI image-scan time by about 90%, a **C++ authentication and authorization service** capable of handling 500+ concurrent sessions with salted SHA-256 hashing, and a **network traffic analyzer and IDS in C** that achieved ~95% detection accuracy using deep packet inspection. Alongside this, I pursued research applying **transformer embeddings to anomaly detection**, benchmarking modern approaches against classical baselines. These experiences strengthened not only my technical depth but also my ability to collaborate through code reviews, secure design practices, and debugging at the system level with tools such as gdb and Valgrind.

Looking forward, I want to contribute to teams that care deeply about **security, systems infrastructure, or ML tooling**, where correctness, observability, and maintainability are valued. My goal is to apply a rigorous engineering mindset to projects that matter—whether in securing software supply chains, scaling backend systems, or developing ML-driven detection frameworks.

---

## Selected Highlights
- Container vulnerability scanner with CVE DB + CIS checks; CI integration reduced detection time by ~90%.
- C++ AuthN/AuthZ service with salted SHA-256; stress-tested to 500+ concurrent sessions; SDL threat model applied.
- C network analyzer & IDS; deep packet inspection rules engine; ~95% detection accuracy.
- Hackathons: CAIDF (Top Finalist) and SparkHacks (Category Winner).

---

## Skills & Keywords
**Languages:** C, C++, Python  
**Systems / Security:** TCP/IP, Linux/WSL, secure coding, IAM, JWT, threat modeling (SDL), input validation, parameterized queries, output encoding  
**Tooling:** Git, CI/CD, gdb, Valgrind, Docker, Kubernetes, Postman, pytest  
**ML:** embeddings, anomaly detection, evaluation pipelines (PyTorch)  

---

## Featured Projects
- [Container Vulnerability Scanner](https://github.com/adit019/container-vuln-scanner) — Python, Docker, CIS checks, CI block on high CVEs
- [Secure AuthZ/AuthN Service](https://github.com/adit019/secure-authz-service-cpp) — C++, salted SHA-256, load testing, SDL mitigations
- [Network Traffic Analyzer & IDS](https://github.com/adit019/network-traffic-analyzer-ids) — C, custom packet capture + rules engine (repo to be made public)
- [Secure Backend API](https://github.com/adit019/secure-backend-api) — Python (Flask), REST, JWT, parameterized queries, automated testing
- [Chess Neural Networks](https://github.com/adit019/uic-chess-nn) — Python, trained models to evaluate chess board states

---

## Contact
- LinkedIn: [linkedin.com/in/adit-sharma-73955a21a](https://linkedin.com/in/adit-sharma-73955a21a)
- Email: **ashar102@uic.edu**

---

## U.S. Presidential Election Data Visualization (1976-2020)

This repository also includes a small, self-contained exploration of U.S. presidential election outcomes from 1976 through 2020. The project packages the source data, a visualization script, and the generated outputs so you can reproduce and extend the analysis locally.

### What’s included
- `data/elections_1976_2020.csv` — Aggregated results with popular vote percentages, Electoral College totals, and third-party vote share.
- `scripts/visualize.py` — Generates charts for major-party popular vote trends, margins, Electoral College outcomes, and third-party vote share. It also exports a markdown summary table to `visualizations/README.md`.
- `visualizations/` — Default output directory for generated PNG charts and the summary markdown table.

### How to run it
1. Create and activate a virtual environment:
   ```bash
   python -m venv .venv
   source .venv/bin/activate
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Generate the charts and summary table:
   ```bash
   python scripts/visualize.py
   ```

All assets will be written to `visualizations/`. The script is intentionally minimal and well-documented so it can serve as a starting point for deeper analysis (e.g., party flips by state or turnout trends).
