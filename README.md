AI Fitness Assessment – Payment Reconciliation System

This project solves a real-world fintech problem where a payment platform’s records do not match bank settlements at month-end. The system identifies discrepancies, explains their causes, and provides a clear reconciliation report.

⚙️ Problem Statement

A payments company records transactions instantly, while the bank settles them after 1–2 days. At month-end, all transactions should match — but they don’t.

This project detects:

Missing settlements
Late settlements
Rounding differences
Duplicate entries
Unknown refunds
🧠 Approach
Generated synthetic transaction datasets (platform + bank)
Performed full outer join reconciliation using Pandas
Applied rule-based detection for different gap types
Produced both summary and detailed reports

🛠️ Tech Stack
Python
Pandas
Jupyter Notebook / Script-based execution
📊 Features
✅ Automatic reconciliation between datasets
✅ Detection of 5 major financial discrepancies
✅ Summary report with issue counts
✅ Detailed transaction-level insights
✅ Tolerance-based amount comparison

⚠️ Limitations (Production Considerations)
May incorrectly flag late transactions due to timezone differences
Does not handle split or partial settlements accurately
Refunds without clear transaction linkage may be misclassified
🚀 Future Improvements
Add Streamlit dashboard for visualization
Integrate real-time transaction processing
Use ML models for anomaly detection
Support partial and many-to-one transaction matching

👨‍💻 Author
Amit Padman
