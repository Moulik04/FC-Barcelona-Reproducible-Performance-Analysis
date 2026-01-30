# FC Barcelona Performance Analysis: Before vs. After Messi

### 1. Project Overview
Evaluated whether Lionel Messi’s 2021 departure had a statistically significant impact on FC Barcelona’s performance metrics, including goals, wins, and points per match.

### 2. Dataset
Season-level and match-level performance data for FC Barcelona, split into two eras: "Before Messi" and "After Messi" (post-2021).

### 3. Approach
* **Tools:** R, R Markdown.
* **Techniques:** Comparative statistical analysis and data visualization using `ggplot2`.
* **Reproducibility:** Optimized the project structure using relative paths and `knitr` configurations.

### 4. Results
* **Metrics:** Average points per match saw a modest dip from **2.18 to 2.16**.
* **Insights:** While there was an immediate performance drop in win rates, recent data indicates a trend of "tactical adaptation," showing that the team is successfully rebuilding its chemistry.

### 5. Key Learnings
The biggest takeaway was the importance of **Project Reproducibility**. I initially struggled with absolute file paths that broke the code on different machines. I solved this by implementing a self-contained folder structure and using `list.files()` with `getwd()`, ensuring the entire analysis could be "knitted" by any user with a single click.
