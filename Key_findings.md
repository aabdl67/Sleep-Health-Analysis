# Sleep Health & Lifestyle Analysis: Key Findings

## Summary
This analysis explored the relationships between sleep patterns, stress, occupation, and health metrics in a sample of `374` individuals. The key insights are summarized below.

## Key Health Metrics from the Dataset
Initial analysis revealed important baseline health statistics for the group:

*   **Average Blood Pressure:** The average blood pressure across the sample was `128.6`/`84.6` mmHg.
*   **Hypertension:** **`2` individuals (`0.53`%)** were found to have systolic hypertension (systolic > 140 mmHg).
*   **Hypotension:** **`0` individuals** were found to have diastolic hypotension (diastolic < 60 mmHg).
*   **Healthy BP:** **`41` individuals (`11.0`%)** had blood pressure in the normal, healthy range (systolic < 120 *and* diastolic < 80).
*   **Blood Pressure Range:** Systolic pressure ranged from `115` to `142` mmHg, while diastolic pressure ranged from `75` to `95` mmHg.

**These figures show that while extreme hypertension is rare in this sample, the average blood pressure is elevated above the ideal healthy range, suggesting potential cardiovascular risk factors.**

## 1. Sleep Duration by Disorder Status
**Finding:** Individuals with sleep disorders get less sleep than those without disorders.

**Details:** The boxplot clearly shows that people with no sleep disorder enjoy the highest median sleep duration (approximately 7-8 hours). Those with Sleep Apnea have a moderately reduced median duration (around 6.5-7 hours), while individuals with Insomnia have the lowest median sleep duration (approximately 5.5-6 hours). This demonstrates a clear link between disordered sleep and reduced sleep quantity.

**Visual Evidence:**

![Sleep Duration by Disorder Status](Viz_Plots/Rplot1_sleep%20duration%20by%20disorder%20status.png)

## 2. Stress vs. Sleep Quality Relationship
**Finding:** There is a strong negative correlation between stress levels and sleep quality.

**Details:** The scatter plot reveals a clear downward trend: as self-reported stress levels increase, reported sleep quality scores consistently decrease. Individuals with the lowest stress (scores 3-5) report high sleep quality (8-9), while those with the highest stress (scores 8-9) report poor sleep quality (4-6). This is one of the strongest relationships in the dataset.

**Visual Evidence:**

![Stress vs. Sleep Quality](Viz_Plots/Rplot2_stress%20vs.%20sleep%20quality.png)

## 3. Occupation-Based Sleep Disorder Prevalence
**Finding:** Certain professions show significantly higher rates of sleep disorders.

**Details:** Sales Representatives and Nurses have the highest proportion of Sleep Apnea cases. Lawyers and Engineers show a higher prevalence of Insomnia. Occupations like Teacher and Accountant appear to have a much lower overall prevalence of sleep disorders. This suggests that job-related factors like stress, shift work, or sedentary behavior may be significant contributors to sleep health.

**Visual Evidence:**

![Sleep Disorders by Occupation](Viz_Plots/Rplot3_sleep%20disorders%20by%20occupation.png)

## 4. Sleep Apnea and BMI Category
**Finding:** Sleep Apnea is overwhelmingly more prevalent among obese individuals.

**Details:** The stacked bar chart provides striking evidence: the proportion of individuals with Sleep Apnea (TRUE) is vastly higher in the "Obese" BMI category compared to all others. The "Normal Weight" and "Overweight" categories consist almost entirely of individuals without Sleep Apnea. This confirms that obesity is the single strongest demographic predictor for this disorder in our sample.

**Visual Evidence:**

![Sleep Apnea vs. BMI Category](Viz_Plots/Rplot4_sleep%20apnea%20vs.%20BMI%20category.png)

## 5. Predictive Model for Insomnia Risk
**Finding:** Stress increases insomnia risk, while physical activity protects against it.
**Details:** A logistic regression model predicts the risk of an Insomnia diagnosis. The results are statistically significant:
- **Stress Level:** Positive coefficient (`0.162`), with a p-value of `0.0295`. For each unit increase in stress, the log-odds of having insomnia increase.
- **Physical Activity Level:** Negative coefficient (`-0.039`), with a highly significant p-value (`<0.001`). For each unit increase in activity, the log-odds of having insomnia decrease.
**This means higher stress levels significantly increase the probability of insomnia, while higher physical activity levels significantly decrease it.**

## Overall Conclusion
This analysis identifies three primary pillars of sleep health:
1.  **Psychological Factors:** **Stress level** is the most significant predictor of sleep quality and a key driver of insomnia risk.
2.  **Physical Health Factors:** **BMI** is the strongest predictor of Sleep Apnea, with obesity dramatically increasing prevalence.
3.  **Behavioral Factors:** **Physical activity** is a major mitigating factor that protects against insomnia, independent of stress levels.

**Occupation** serves as an important overlay, likely influencing all three pillars (e.g., a high-stress job increases stress, a sedentary job reduces activity). The elevated average blood pressure in the sample further suggests that sleep, cardiovascular, and metabolic health are deeply interconnected. Interventions aimed at improving sleep should therefore adopt a holistic approach, targeting weight management, stress reduction, and the promotion of physical activity simultaneously.
