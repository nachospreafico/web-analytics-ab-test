# A/B Testing — Web Analytics Signup Experiment

## Overview

This project presents an **end-to-end A/B testing analysis** using Python, framed around a realistic **web analytics** use case.  
The goal is to evaluate whether a new website design improves the **user signup rate** compared to the current design.

The project is designed to mirror how a **Product / Growth Analyst** would approach experimentation in a real company: from business framing and experiment design to statistical analysis and decision-making.

---

## Business Problem

The company wants to decide whether to **ship a new website design** based on its impact on user signups.

**Primary question:**  
Does the new design increase the signup conversion rate compared to the current design?

---

## Experiment Design

- **Variants**
  - Control (A): current website design
  - Variant (B): new website design
- **Unit of analysis:** user
- **Primary metric:** signup rate (signups / visitors)
- **Assignment:** users are randomly assigned to one variant and exposed to only that version

---

## Dataset

The dataset was **synthetically generated** to simulate a real-world A/B test.

### Schema

- `user_id`: unique identifier per user
- `variant`: Control (A) or Variant (B)
- `converted`: whether the user signed up (0/1)
- `session_duration`: session length in seconds
- `device`: device type (mobile, desktop, etc.)
- `traffic_source`: acquisition channel

Conversion probabilities are intentionally close between variants to reflect realistic product experiments where effects are typically small.

---

## Methodology

1. Data generation and validation
2. Sanity checks and exploratory analysis
3. Two-proportions z-test for conversion comparison
4. Effect size estimation (absolute and relative lift)
5. Confidence interval interpretation
6. Business recommendation

---

## Key Takeaways

- Statistical significance alone is not sufficient — effect size and uncertainty matter.
- Confidence intervals help assess potential upside and downside risk.
- The final recommendation balances statistical evidence with business judgment.

---

### Screenshots

##### Summary

[A/B Test Summary Table](/images/summary.png)

## Tech Stack

- Python
- pandas
- numpy
- scipy
- matplotlib
- seaborn

---

## How to Run

1. Clone the repository
2. (Optional) Create a virtual environment
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Open and run the Jupyter notebook

---

## Final Recommendation

Based on the experiment results, the new website design shows a meaningful and statistically supported improvement in signup rate.  
The recommended action is to **ship the new design**, while continuing to monitor performance post-deployment.

---

## Notes

This project is intended for **portfolio and interview demonstration purposes**, showcasing analytical thinking, experimentation best practices, and clear business communication.

## 📬 Contact

**Ignacio Spreafico**  
Data & Business Analyst | Driving Decisions with Python, SQL & Power BI | Statistics & Machine Learning

📧 Email: **nachospreafico06@gmail.com**  
🔗 LinkedIn: **https://www.linkedin.com/in/ignacio-spreafico**  
🐙 GitHub: **https://github.com/nachospreafico**

---

## ⭐ Support / Feedback

If you like this project, consider leaving a ⭐ on GitHub!  
This project is part of my data science portfolio and demonstrates statistical reasoning, product analytics thinking, and clean code practices.
