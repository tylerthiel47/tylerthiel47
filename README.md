tylerthiel/README.md

# Tyler Thiel

M.S. Business Analytics candidate at Wake Forest (May 2026), B.A. from Furman. I like the parts of analytics that most people skip past to get to the model — figuring out what question actually matters, cleaning up data that's lying to you, checking whether the output would survive someone asking "why" three times in a row.

Most of what's below is coursework and side projects. The tennis work is real but the underlying data belongs to the program, so I've described it without the code.

Python, R, SQL, Power BI, Tableau, Excel, Alteryx, Git

## Background

- M.S. Business Analytics, Wake Forest University School of Business — May 2026
- B.A. Business Administration (Finance & International Business), minor in Business Analytics, Furman University — May 2025
- Graduate Consultant, Wake Forest Men's Tennis, Oct 2025–present. Built a metric the coaching staff uses to gauge how players perform under pressure, using four seasons of match data plus their own qualitative notes from practice and film sessions.
- Ticket Sales Intern, Greenville Swamp Rabbits, 2023–2024. Mostly cold outreach and season-ticket sales, but the promotions I helped run correlated with a big jump in attendance that year.
- Bloomberg Market Concepts, Alteryx Foundation certs

## How I work

I try to write down the actual decision a project is supposed to inform before I touch any data — otherwise it's easy to end up with a model that's technically fine and answers nothing anyone asked. The fraud detection project below is a good example of this going sideways at first: I had a decent-looking classifier that was basically useless because I hadn't thought hard enough about what a false negative actually costs versus a false positive.

I also use Claude a fair amount, mostly for scaffolding SQL or debugging something at 1am, but I try to be the one who decides the actual approach and checks the output makes sense before I trust it.

## Selected work

**customer-churn-prediction** — classification model to flag customers likely to churn, built on tenure/billing/support data. Tried a few model types before landing on gradient boosting; tuned for recall since a missed churner is more expensive than a false alarm. [repo](https://github.com/tylerthiel/customer-churn-prediction)

**sales-performance-dashboard** — Power BI dashboard that replaced a manual Excel report someone was rebuilding every week by hand. Star schema, a handful of DAX measures, drill-down from company-wide KPIs down to individual rep numbers. [repo](https://github.com/tylerthiel/sales-performance-dashboard)

**ff3-factor-model** — Fama-French three-factor regression pipeline in Python. Pulls prices and Ken French's factor data, runs the regression, ranks multiple tickers against each other. Has a self-check step that flags multicollinearity and bad joins before it trusts its own output. [repo](https://github.com/tylerthiel/ff3-factor-model)

**Resilience Index (Wake Forest Tennis, no public code)** — a stress-performance metric for the tennis team, combining match stats with coaching input. Used K-Means to split players into three rough archetypes (aggressive, rally-based, clutch) that the staff now uses to shape training.

**Deacon Financial Services Fraud Detection (coursework)** — imbalanced-data fraud model, logistic regression baseline then a class-weighted random forest. Learned more from getting the validation setup wrong the first time than from the final model.

**Capsim Business Simulation (coursework)** — multi-round business sim, my group ended up winning our section. I mostly handled financial forecasting and R&D allocation.

---

tcthiel@outlook.com · [linkedin.com/in/tyler-thiel](https://linkedin.com/in/tyler-thiel/)
