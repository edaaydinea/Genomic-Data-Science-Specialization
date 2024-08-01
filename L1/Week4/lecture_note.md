# Why Care About Statistics?

- **Components of Genomic Data Science:**
    - Comprises biology, computer science, and statistics.
    - Statistics often perceived as the lesser component.
- **Significance of Statistics:**
    - Vital for genomic data science, often overlooked compared to biology and computer science.
- **Case Study - Personalized Cancer Therapy:**
    - A significant result published in *Nature Medicine* suggested genomic measurements could predict effective chemotherapies for individuals.
    - Seen as a "holy grail" in personalized cancer therapy.
- **Reproduction of Results:**
    - MD Anderson Cancer Center attempted to reproduce the results.
    - Statisticians Keith Baggerly and Kevin Coombes led the effort.
    - Encountered issues with data transparency and reproducibility.
- **Outcome and Scandal:**
    - Inability to reproduce results led to a scandal in genomic data science.
    - Clinical trials initiated based on flawed data analysis.
    - Resulted in lawsuits involving patients and Duke University.
- **Institute of Medicine Report:**
    - Triggered a report focusing on new standards for developing genomic data technologies.
    - Emphasized statistical issues, reproducibility, and model development.
- **Examples Highlighting the Importance of Statistics:**
    - Published paper abstract with placeholder for "insert statistical method here," indicating neglect of statistical importance.
    - Berkeley flyer listing statistics without an application area, suggesting underappreciation of its role.
- **Conclusion:**
    - A lack of statistical thinking can lead to significant issues in genomic data analysis.
    - It is crucial to emphasize statistics equally alongside biology and computer science in genomic data science.

# What Went Wrong?

- **Motivation from Previous Lecture:**
    - Highlighted problems in an analysis using genomic measurements to determine appropriate chemotherapies.
    - Two main reasons for failure: lack of transparency and lack of expertise.
- **Lack of Transparency:**
    - **Data and Code Availability:**
        - Raw and processed data, as well as the code used for analysis, were not accessible.
        - This hampered reproducibility, preventing others from verifying the results.
    - **Cooperation Issues:**
        - The original authors were reluctant to share data and code with others, including statisticians.
- **Lack of Expertise:**
    - **Statistical Expertise:**
        - The analysis involved incorrect and "silly" prediction rules, such as inappropriate probability definitions.
    - **Study Design Problems:**
        - Experimental design flaws included confounders, like running samples on different days, affecting outcomes.
    - **Unstable Predictions:**
        - Prediction rules included random components, leading to different treatment recommendations on different days despite the same data and code.
        - Inconsistencies were not due to data or algorithm changes but timing of algorithm execution.
- **Consequences and Lessons:**
    - The analysis was ultimately reproducible but fundamentally flawed due to incorrect data analysis.
    - A critical lack of statistical expertise led to these issues, highlighting the importance of sound statistical knowledge in genomic data science.
- **Conclusion:**
    - Proper statistical expertise is crucial for designing studies, creating accurate statistical procedures, and avoiding major issues in genomic data analysis, as demonstrated by the Duke scandal.

# The Central Dogma of Statistics

- **Central Dogma of Statistics:**
    - Explains the primary goal of the field: understanding a population based on a sample.
    - Similar to biology's central dogma, but focuses on statistical inference.
- **Problem of Population Measurement:**
    - Measuring an entire population can be impractical due to cost or difficulty.
    - The goal is to make inferences about the population without measuring every individual.
- **Sampling and Probability:**
    - A small, probabilistic sample is taken from the population to represent it.
    - The sample should ideally reflect the larger population.
- **Example of Sampling:**
    - Consider a population with pink and gray symbols.
    - A sample might contain two pink and one gray symbol.
    - From this sample, an inference can be made about the overall proportion of pink and gray symbols.
- **Statistical Inference:**
    - Involves making educated guesses about the population based on the sample.
    - Includes estimating the population characteristics and the variability of these estimates.
- **Importance of Variability:**
    - A sample's representation of the population can vary, leading to potential estimation errors.
    - It is crucial to quantify this variability to understand the accuracy of the inferences.
- **Changing Populations:**
    - If the population changes after sampling (e.g., introduction of purple symbols), the sample may no longer represent it accurately.
    - This can affect the validity of the inference.
- **Example of Changing Population - Google Flu Trends:**
    - Used search terms to predict flu activity.
    - Initially successful, but later failed due to changes in how people searched for flu symptoms.
    - The population's search behavior had changed, making the initial model inaccurate.
- **Summary:**
    - The central dogma of statistics involves using a sample to infer information about a population.
    - Key considerations include the sample's representativeness and the variability of estimates.
    - Awareness of potential changes in the population is crucial for accurate statistical inference.

# Data Sharing Plus

- **Importance of Data Sharing:**
    - Transparency in data sharing is crucial for reproducibility and validation.
    - A comprehensive data sharing plan ensures that others can access and analyze the data.
- **Components of a Data Set:**
    - A complete data set consists of four key components:
        1. **Raw Data:** The unprocessed, original data. In genomics, this could include sequencing reads in formats like FASTQ, BAM files, or even images underlying the sequence data.
        2. **Tidy Data Set:** A processed and cleaned version of the raw data, organized for analysis. It follows the structure of one variable per column, one observation per row, and one table per data set type, with linking indicators if multiple data sets are used.
        3. **Code Book:** Describes the variables in the tidy data set, including their names, descriptions, and units. It is essential for understanding the data, especially to avoid misunderstandings like those caused by unit discrepancies.
        4. **Recipe:** A detailed description of the steps taken to transform the raw data into the tidy data set. This should ideally be in the form of a script (e.g., written in R or Python) that can be run without manual intervention. Alternatively, a detailed list of instructions can be provided, but it requires meticulous documentation.
- **Raw Data:**
    - Must be untouched and unprocessed to retain its original state.
    - What constitutes "raw data" may vary depending on the context and the stage at which the data is received.
- **Tidy Data Set:**
    - Structured data that is easy to analyze and work with.
    - Should include all relevant variables and observations, organized in a clear and consistent manner.
- **Code Book:**
    - Provides essential metadata about the data set, including variable definitions and units.
    - Helps prevent confusion and errors, such as those caused by using different measurement units.
- **Recipe for Data Processing:**
    - A script is the preferred method for documenting the data transformation process, as it can be executed automatically without ambiguity.
    - If a script is not feasible, an exhaustive list of steps, software versions, parameters, and even videos (for actions taken in software like Excel) must be provided.
- **Recommendations for Data Sharing:**
    - Use scripts wherever possible to ensure reproducibility.
    - Avoid vague instructions and ensure all necessary details are included.
    - A data sharing plan template is available on GitHub, offering guidance on sharing data effectively and transparently.

# Getting Help with Statistic

- **Importance of Statistics in Genomic Big Data Science:**
    - Statistics play a crucial role in analyzing and interpreting large-scale genomic data. Understanding statistical methods is essential for making valid inferences and decisions based on this data.
- **Ways to Learn and Get Help in Statistics:**
    - **Self-Learning:**
        - There are many online resources and courses available for learning statistics, including specializations that focus on data science and include statistical components.
        - Examples include courses offered by Johns Hopkins University, which provide comprehensive training in statistics and data science.
    - **Q&A Sites:**
        - Websites like Cross Validated and Stack Overflow are valuable resources for asking specific questions about statistical analyses or software packages. These platforms can help with issues related to model fitting, interpretation, and other statistical challenges.
- **Seeking Expert Help:**
    - **Lonely Bioinformatician:**
        - A bioinformatician hired to work in a biology lab without the support of a broader computational community. While some excel in this role, it can be challenging due to limited access to resources and expertise.
    - **Long-Term Collaborations:**
        - Collaborating with a center for computational biology or biostatistics is often the most effective way to access deep statistical and computational expertise. These centers typically bring together professionals from various fields, including biology, biostatistics, and computer science, to address complex computational biology problems.
        - At institutions like Johns Hopkins, centers for computational biology offer a collaborative environment where genomic data scientists work together on advanced analyses.
- **Advantages of Collaborations:**
    - Collaborations with established centers provide access to a wealth of knowledge, resources, and support, facilitating more comprehensive and accurate analyses.
    - Long-term collaborations foster deeper understanding and innovation in tackling statistical and computational challenges in genomics.

# Plotting Your Data

- **Interactive Analysis and Plotting:**
    - **Importance of Plotting:**
        - Visualizing genomic data through plots is crucial for understanding the data's characteristics and properties. It helps summarize large datasets, making them more manageable and easier to interpret.
    - **Making Big Data Small:**
        - The concept, attributed to Robert Gentleman, emphasizes the need to reduce the complexity of large datasets into simpler, more understandable forms. This process involves summarizing the data just enough to allow effective visualization and exploration.
- **Example of Misleading Statistical Summaries:**
    - **Identical Summary Statistics, Different Patterns:**
        - An example is given where four different datasets have identical summary statistics (such as slope coefficients and correlation coefficients) but display vastly different patterns when plotted. This highlights the limitations of relying solely on summary statistics without visual inspection.
- **Effective Visualization Techniques:**
    - **Detailed Plots vs. Simplified Plots:**
        - A comparison is made between a "bad" plot, which shows bar plots with confidence bounds but no raw data, and a "good" plot, which includes both summary statistics and raw data points. The latter provides more transparency and allows for a better understanding of the data distribution.
    - **Plotting Replicates:**
        - When comparing technical replicates, it is important to consider the scale and distribution of data. Using transforms, such as log transformation, can help spread out tightly clustered data, making patterns more discernible.
    - **Bland-Altman Plot (MA Plot):**
        - Instead of plotting one replicate against another, the Bland-Altman plot (or MA plot) is used. This plot displays the average expression levels (sum of replicates) on the x-axis and the difference between replicates on the y-axis. It helps identify trends and discrepancies, particularly useful for identifying variability in lowly expressed genes.
- **Caution Against Misleading Visuals:**
    - **Ridiculograms:**
        - The term "ridiculogram" refers to visually appealing network plots that may lack substantive scientific information. While aesthetics are important, the primary goal of statistical graphics should be to communicate scientific information clearly and accurately.

# Sample Size and Variability

- **Central Dogma of Statistics:**
    - **Population vs. Sample:**
        - Due to the high cost of measuring entire populations, samples are taken to make inferences about the population.
    - **Statistical Inference:**
        - Beyond estimating the central tendency (mean) from a sample, it’s crucial to estimate the variability to understand the uncertainty and reliability of the conclusions drawn.
- **Sample Size Determination:**
    - **Basic Formula:**
        - Sample size $N$ can be calculated as the budget divided by the cost per measurement. However, this method doesn’t necessarily reflect the optimal sample size for detecting effects.
    - **Importance of Variability:**
        - The primary goal in determining sample size is to understand and account for the variability in the data. The difference in means between groups and the variability around these means are key considerations.
- **Power Analysis:**
    - **Concept of Power:**
        - Power is the probability of detecting a real effect if it exists. It depends on the sample size, the difference between group means, and the variability within the data.
    - **Calculation Example:**
        - For a given effect size and variability, power calculations can determine the necessary sample size to achieve a desired power level (commonly 80%). For instance, detecting an effect size of 5 with a standard deviation of 10 and aiming for 80% power may require 64 samples per group.
- **Types of Variability:**
    - **Phenotypic Variability:**
        - Differences between groups (e.g., cancer vs. control) in genomic measurements.
    - **Measurement Error:**
        - Variability due to the limitations of genomic measurement technologies.
    - **Natural Biological Variation:**
        - Inherent variability among individuals, even under similar conditions. This type of variability must be accounted for in statistical modeling.
- **Considerations in Genomic Studies:**
    - **Technical vs. Biological Variability:**
        - New technologies may reduce technical variability (measurement error) but do not eliminate natural biological variation.
    - **Visual Example:**
        - A comparison of next-generation sequencing (NGS) and microarray technologies shows that while technical variability may differ, biological variability remains consistent across technologies.
- **Concluding Thoughts:**
    - Understanding and accounting for variability in both samples and populations is critical in designing genomic studies. Proper sample size determination and power analysis are essential to ensure reliable and valid conclusions.

# Statistical Significance

- **Concept of Statistical Significance:**
    - **Objective:** Determine if observed differences in sample measurements are replicable and indicate a real effect in the population.
    - **Real Difference:** Typically refers to differences in mean values between groups, considering variability.
- **Examples of Data and Variability:**
    - **Gene Expression Data:**
        - **Gene 1:** Small difference in means but high variability; hard to conclude a significant difference.
        - **Gene 2:** Clear difference with tightly clustered data points; suggests a significant difference.
        - **Gene 3:** Apparent difference with similar variability and mean values; may or may not be significant.
- **T-Statistic:**
    - **Definition:** Measures the difference between group means relative to the variability of measurements.
    - **Formula:**  $t=\frac{\bar{Y} - \bar{X}}{\sqrt{\frac{S^2_Y}{n_Y} + \frac{S^2_X}{n_X}}}$
        - $\bar{Y}$ and $\bar{X}$ are sample means.
        - $S^2_Y$ and $S^2_X$ are sample variances.
        - $n_Y$ and $n_X$ are sample sizes.
    - **Interpretation:** Larger t-values indicate greater likelihood of a real difference.
- **P-Values:**
    - **Definition:** Probability of observing a statistic as extreme or more extreme than the calculated value, given that the null hypothesis (no difference) is true.
    - **Permutation Test:**
        - Scramble group labels, recalculate statistics, and create a distribution of these statistics.
        - The p-value is the proportion of scrambled statistics that are more extreme than the observed statistic.
    - **Common Cutoff:** p-value < 0.05 is often considered statistically significant.
- **Misinterpretations of P-Values:**
    - **Not a Probability of the Null Hypothesis Being True:** P-value does not indicate the probability that the null hypothesis is true.
    - **Not a Probability of the Alternative Hypothesis Being True:** P-value does not measure the likelihood of the alternative hypothesis.
    - **Not a Measure of Evidence:** It’s not a direct measure of how much evidence supports or contradicts a hypothesis.
- **Issues and Misuses:**
    - **Cutoff Controversy:** The 0.05 cutoff is arbitrary and widely adopted without strong rationale.
    - **Over-interpretation:** Misuse and misunderstanding of p-values contribute to issues in statistical reporting and interpretation.
- **Practical Implications:**
    - **Power of the Study:** Consideration of sample size and variability is crucial in determining statistical power and ensuring robust conclusions.
    - **Critical Thinking:** Avoid over-relying on p-values and understand their limitations.

# Multiple Testing

- **Multiple Testing Issue:**
    - **Context:** In genomic studies, researchers often conduct thousands to millions of tests simultaneously, such as comparing gene expressions or DNA variants across groups.
    - **Challenge:** Standard hypothesis testing frameworks and p-values, which are designed for single tests, become problematic when applied to multiple tests.
- **Uniform Distribution of P-Values:**
    - **When No Signal Exists:** If there is no real effect, p-values are uniformly distributed. This means:
        - 5% of p-values will be less than 0.05.
        - 20% of p-values will be less than 0.02, and so on.
    - **Implication:** When performing many tests, even in the absence of a true effect, some p-values will fall below the significance threshold by chance alone.
- **Example Scenario:**
    - **Jelly Beans and Acne Study:** Performing multiple tests on different types of jelly beans might yield at least one p-value below 0.05 purely by chance, leading to misleading conclusions about significance.
- **Error Rates for Multiple Testing:**
    - **Family-Wise Error Rate (FWER):** Controls the probability of making at least one false positive among all tests.
        - **Very Strict:** Requires that the probability of even one false positive is very low.
    - **False Discovery Rate (FDR):** Controls the proportion of false positives among the discoveries made.
        - **More Liberal:** Allows some false positives to make more discoveries, but quantifies their expected proportion.
- **Comparison of Error Rates:**
    - **Thresholding P-Values:** If using a 0.05 threshold, about 5% of results are expected to be false positives. For 10,000 tests, this could mean 500 false positives among 550 significant findings.
    - **Using FDR:** For the same 550 significant findings, with a 5% FDR, the expected number of false positives would be about 27.5.
    - **Using FWER:** Ensures that the probability of having even one false positive among the 550 findings is less than 0.05, implying most findings are likely true positives.
- **Avoiding Misinterpretation:**
    - **Different Interpretations:** FDR and FWER provide different views on error control, and results can vary based on which error rate is used.
    - **Publication Bias:** Negative results (p-value > 0.05) should be reported to avoid bias and maintain scientific integrity.
- **Avoiding P-Value Hacking:**
    - **P-Value Hacking:** Altering analysis methods to achieve statistically significant results.
    - **Best Practice:** Develop a data analysis plan before examining data and adhere to it to avoid manipulating results.
- **Summary:**
    - **Multiple Testing:** Requires adjustment of error rates to ensure accurate and reliable findings.
    - **Error Rate Metrics:** FWER and FDR help manage the balance between discovering true effects and controlling false positives.
    - **Scientific Integrity:** Avoid manipulating data or analyses to achieve significance and report all results honestly.

# Study Design, Batch Effects, and Confounding

1. **Confounding:**
    - **Definition:** A confounder is a variable that is related to both the independent variable (e.g., shoe size) and the dependent variable (e.g., literacy) and can create a misleading association between them.
    - **Example:** In the context of shoe size and literacy:
        - **Observation:** It might seem that larger shoe sizes are associated with higher literacy.
        - **Reality:** The actual confounding factor is age, which affects both shoe size and literacy. Younger individuals have smaller shoes and lower literacy, while older individuals have larger shoes and higher literacy.
    - **Impact:** Confounders can distort the perceived relationship between variables and lead to incorrect conclusions.
2. **Batch Effects:**
    - **Definition:** Batch effects are systematic differences in measurements due to variations in the conditions under which samples were processed, rather than true biological differences.
    - **Example 1:** A study comparing gene expression between ethnic groups found a large number of differentially expressed genes. However, it was later revealed that the samples were collected in different years, introducing a batch effect.
    - **Example 2:** Another study on SNPs and longevity was retracted because it used different technologies for younger and older individuals, creating batch effects.
    - **Impact:** Batch effects can lead to spurious findings and incorrect interpretations if not properly accounted for.
3. **Addressing Confounding and Batch Effects:**
    - **Randomization:**
        - **Purpose:** Randomly assigning treatments or conditions to participants helps break any relationship between the treatment and confounding variables.
        - **Example:** Randomly assigning patients to different treatments (red or green) regardless of their age or other confounding factors ensures that these factors do not bias the results.
    - **Stratification:**
        - **Purpose:** Designing the experiment to account for known confounders by ensuring that each confounder is evenly represented across different treatment groups.
        - **Example:** In an experiment with mice, both treated and control groups should be balanced for factors like sex and time, ensuring that both groups are equally exposed to these potential confounders.
4. **Good Experimental Design:**
    - **Balance:** Ensure equal numbers of treated and control samples to avoid imbalance.
    - **Replication:**
        - **Technical Replicates:** Repeat experiments with the same sample to assess technology reliability.
        - **Biological Replicates:** Use samples from different individuals to measure biological variability.
    - **Controls:**
        - **Negative Controls:** Confirm that no effect is due to experimental artifacts.
        - **Positive Controls:** Ensure that the experimental design and technology are functioning correctly.
5. **Key Takeaways:**
    - **Avoid Misinterpretation:** Be aware of potential confounders and batch effects that might skew results.
    - **Design Carefully:** Use randomization and stratification to minimize confounding effects and ensure robust experimental design.
    - **Report Honestly:** Address and report any potential sources of bias or error in your study to maintain scientific integrity.

By accounting for confounding factors and batch effects, researchers can produce more reliable and interpretable results, leading to valid conclusions in genomic studies and other scientific research.