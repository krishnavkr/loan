# Smart Loan Recovery System
built a loan recovery system with Machine Learning, using dataset containing borrower profiles, loan details, and repayment histories. This dataset includes critical attributes such as:

1. **Demographic Information:** Age, employment type, income level, and number of dependents.
2. **Loan Details:** Loan amount, tenure, interest rate, and collateral value.
3. **Repayment History:** Number of missed payments, days past due, and monthly EMI payments.
4. **Collection Efforts:** Collection methods used, number of recovery attempts, and legal actions taken.
5. **Loan Recovery Status:** Whether the loan was fully recovered, partially recovered, or remains outstanding.

**Defined a function that categorizes borrowers into three recovery approaches:**

*   Immediate legal action for high-risk borrowers (risk score > 0.75).
*   Settlement offers and repayment plans for moderate-risk borrowers (0.50 – 0.75).
*   automated reminders for low-risk borrowers (<0.50).

This function was applied to the test dataset to assign a personalized recovery strategy to each borrower to ensure cost-effective and targeted loan recovery efforts.






**--- Model Performance Comparison ---**

Random Forest:
* Accuracy: 0.9200
* Precision (High Risk): 0.9500
* Recall (High Risk): 0.9194
* F1-Score (High Risk): 0.9344
*  AUC: 0.9854

XGBoost:
 * Accuracy: 0.9400
 * Precision (High Risk): 1.0000
 * Recall (High Risk): 0.9032
 * F1-Score (High Risk): 0.9492
 * AUC: 0.9911

**Conclusion:**

Based on the AUC score, XGBoost appears to be the better performing algorithm for this task.
It achieves a higher AUC, indicating a better ability to distinguish between high-risk and non-high-risk loans.
XGBoost also has a higher F1-score for the 'High Risk' class, suggesting a better balance between precision and recall for identifying high-risk loans.




