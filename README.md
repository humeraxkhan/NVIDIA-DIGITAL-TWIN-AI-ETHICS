# AI Ethics Digital Twin System

A simulation system designed to model, detect, and predict ethical risks in automated industrial environments, combining machine learning, ethical auditing, and formal verification.

---

## Overview

This project simulates a digital twin environment in which workers interact with automated systems. The primary goal is to identify and prevent ethical violations that arise when industrial automation is deployed without adequate safeguards.

The system addresses four core ethical concerns:

- Privacy violations arising from worker monitoring without informed consent
- Failure to notify workers when automation affects their roles
- Absence of retraining support for workers displaced by automation
- High-energy computational usage without appropriate oversight and review

To address these concerns, the system integrates three complementary components: a machine learning model for ethical risk prediction, an ethical auditing layer for detecting violations, and a formal verification module using the Z3 SMT solver to mathematically enforce ethical constraints.

---

## Features

- Simulation of worker behaviour in automated digital twin environments
- Detection and quantification of ethical violations across multiple categories
- Random Forest classifier for predicting worker ethical risk
- Environmental impact simulation tracking computational energy usage
- Formal verification of ethical rules using the Z3 solver
- Visualisation of audit results including risk distribution and violation breakdowns

---

## Project Structure

```
ai-ethics-digital-twin/
├── our_code_for_ethics_report.ipynb
├── requirements.txt
└── README.md
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/ai-ethics-digital-twin.git
cd ai-ethics-digital-twin
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Usage

Launch the Jupyter Notebook environment:

```bash
jupyter notebook
```

Open the following file to run the full simulation and verification pipeline:

```
our_code_for_ethics_report.ipynb
```

---

## Machine Learning Model

A Random Forest Classifier is trained to predict ethical risk for each simulated worker based on the following features:

- Consent status
- Monitoring activity
- Automation impact
- Notification status
- Retraining availability

The model achieves approximately 83% accuracy in predicting ethical risk scenarios across the simulated dataset.

---

## Ethical Rules and Formal Verification

The Z3 SMT solver is used to encode and verify four key ethical constraints:

- Workers must not be monitored without giving informed consent
- Workers affected by automation must be notified of the impact
- Retraining support must be provided to workers displaced by automation
- Simulation runs classified as high-energy must trigger a formal review process

When the solver returns **UNSAT**, the ethical property holds under the encoded system constraints and no violation is possible. When the solver returns **SAT**, a counterexample has been found indicating a violation of the specified constraint.

---

## Example Outputs

- Worker audit summary with violation counts across all ethical categories
- Risk distribution across the simulated workforce
- Ethical violation breakdown visualised as a bar chart
- Environmental audit summary tracking high-energy simulation runs

---

## Key Insight

This project demonstrates how ethical principles can move beyond abstract discussion into concrete, verifiable system constraints. By encoding fairness, consent, and accountability as logical properties, the system provides a mechanism for detecting, predicting, and formally proving ethical compliance in automated environments — rather than relying on high-level claims that remain untested.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Z3 Solver

---

## Future Improvements

- Integration with real-world industrial datasets
- Interactive monitoring dashboard using Streamlit
- Extension to more advanced machine learning models such as XGBoost or neural networks
- Real-time monitoring and alerting system for live ethical risk detection

---

## Authors

**Humera Khan**
MSc Advanced AI, University College Dublin

**Aisling Wallace**
MSc Advanced AI, University College Dublin

---

## Acknowledgements

- NVIDIA Omniverse — conceptual inspiration for the digital twin simulation framework
- UCD School of Computer Science — academic supervision and support
- Dr. Vivek Nallur — project supervisor

