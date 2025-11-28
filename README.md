# My Analytics Application Experience

Welcome! 👋 This is my midterms portfolio for CIS221 — a collection of my hands-on work with data analytics, statistical analysis, and machine learning concepts.

---

## What's In Here?

### Core Analytics Work
- **Correlation Practice Part 1, 2, & 3.ipynb** - My journey understanding how variables relate to each other. Sounds simple, but it's deceptively nuanced once you get into multicollinearity and non-linear relationships.
- **Data Cleaning through Imputation Techniques.ipynb** - Real talk: most analytics work is actually just data cleaning. This notebook covers the different ways to handle missing data without messing up your analysis.
- **Loading, Organizing, Storing Data 1 & 2.ipynb** - Practical exercises on setting up data pipelines properly. Think of it as the foundation for any BI project.
- **Quick Descriptives One.ipynb** - Summarizing data effectively. Useful for creating dashboards and business reports.

All of these follow the **CRISP-DM Framework**, which is basically the standard roadmap for any data project in IS.

---

## What Actually Happened During Midterms?

### The Real Challenges I Faced

**1. Data is Messy (and Nobody Tells You How Messy)**

When I started working with real datasets, I quickly realized that data quality is *the* biggest bottleneck. I spent way more time cleaning data than I expected:
- Missing values everywhere (and no clear reason why they were missing)
- Outliers that seemed like errors but actually meant something important
- Inconsistent formats and data entry mistakes
- Choosing between different imputation methods without knowing which was "correct"

**2. Correlation ≠ Causation (and It's Harder to Remember Than You'd Think)**

This sounds like common knowledge, but when you're looking at correlation coefficients, it's easy to fall into the trap of interpreting them causally. I realized that:
- High correlations can be coincidental
- Confounding variables hide the real relationships
- Sometimes you need domain knowledge (talking to business stakeholders) to interpret results properly
- Tools don't substitute for critical thinking

**3. Machine Learning Models Are Overconfident**

Building a model that gets 95% accuracy on training data feels amazing... until you test it on new data and it tanks. I learned the hard way that:
- High accuracy during training often means overfitting, not a good model
- You need proper validation strategies (cross-validation, holdout test sets)
- Different metrics matter (accuracy isn't everything—sometimes precision or recall matters more)
- Simplicity often beats complexity

---

## Why Did This Happen?

### The Root Causes (With Some Theory)

**On Data Quality:**
Real-world data doesn't follow textbook assumptions. From an IS perspective, this usually comes down to:
- Legacy systems with poor data governance
- Manual data entry errors accumulating over time
- Missing documentation on data collection methods
- Integration issues when combining data from multiple sources

Understanding these IS fundamentals helped me appreciate why data preparation is so critical in analytics projects.

**On Statistical Interpretation:**
Most correlation scenarios have hidden complexity:
- **Simpson's Paradox** - trends reverse when you disaggregate data
- **Confounding Variables** - external factors create false relationships
- **Selection Bias** - the data you're seeing isn't representative

This is especially important when working on BI projects—misinterpreting data can lead to bad business decisions.

**On Model Performance:**
Machine learning models optimize for training data, not real-world performance. The techniques that help combat this (regularization, cross-validation, ensemble methods) all exist because of this fundamental tension. It's not something you can just ignore.

---

## What I'm Taking Away & Doing Differently Next Time

### Key Lessons

✅ **Data Governance Matters More Than Model Complexity**
- Before touching a model, invest in understanding and documenting the data
- Create data dictionaries and quality checks upfront (especially relevant as an IS student)
- Automate data profiling to catch issues early

✅ **Always Talk to the Business**
- What problem are we actually solving?
- What decisions will this analysis inform?
- What metrics actually matter to stakeholders?

✅ **Reproducibility is Not Optional**
- Document everything: assumptions, data sources, preprocessing steps, random seeds
- Version control matters for data just as much as code
- Future you (or a colleague) will thank you

✅ **Simple Often Beats Clever**
- A linear regression that you can explain is better than a black-box model that's slightly more accurate
- Stakeholders need to trust your analysis—interpretability helps with that
- Technical debt from over-complicated solutions slows you down later

### What I'll Do Better Next Time

1. **Start with a Data Audit** - Profile the dataset completely before analysis. Create automated quality reports.

2. **Feature Engineering with Purpose** - Don't just throw everything into a model. Think about what variables actually matter for the business problem.

3. **Multiple Validation Approaches** - Use stratified k-fold cross-validation, holdout sets, and business-relevant metrics. Not just accuracy.

4. **Build Interpretable Models First** - Get your baseline with something simple and interpretable. Only add complexity if needed.

5. **Document the "Why"** - Comments in code are fine, but I should write out the analytical decisions: Why did I choose this imputation method? Why are we using this feature? This helps with model governance and auditing.

6. **Stakeholder-Ready Outputs** - Notebooks are great for development, but final deliverables should be dashboards, reports, or visualizations that non-technical people can understand.

---

## The Technical Stack

- **Python** - For all the actual analysis
- **Jupyter Notebooks** - Where the experimentation happens
- **Pandas & NumPy** - Data manipulation and numerical work
- **Scikit-learn** - Machine learning algorithms
- **Matplotlib & Seaborn** - Visualizations for exploration
- **SciPy** - Statistical testing

For real projects, I'd integrate this with **Power BI** or **Streamlit** for dashboards, and **PostgreSQL** or **Flectra** for data storage and management.

---

## How to Navigate This Repo

1. Start with the **EDA notebooks** (Correlation Practice series) to see how I explored the data
2. Check out the **Data Cleaning** notebook to see my imputation decisions
3. Review the **Data Management** notebooks for pipeline practices
4. Read the comments in each cell—I tried to explain my thinking throughout

Each notebook is independent, so you can pick any one and run it without dependencies.

---

## Honest Reflection

This assignment helped me realize that analytics isn't just about algorithms and statistics—it's about understanding systems, data quality, and business problems. As an IS student, I appreciate how these notebooks connect to real database design, data governance, and BI strategy.

The challenges I faced aren't failures; they're exactly what taught me the most. Next time I work on a project (whether for class or professionally), I'll have these lessons embedded in my process.

---

**Course:** CIS221  
**Assignment:** Journal 1 - Analytics Application Experience  
**Framework:** CRISP-DM  
**Created:** November 2025

**License:** GPL-3.0

---

Feel free to reach out if you have questions about any of this work or want to discuss the concepts further. Always happy to talk data! 📊
