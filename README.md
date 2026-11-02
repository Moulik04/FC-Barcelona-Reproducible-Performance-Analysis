# FC Barcelona Performance Analysis: Before vs. After Messi

### 1. Project Overview
Compared FC Barcelona's La Liga results in the three seasons before Lionel Messi left (2018/19 to 2020/21) with the three after (2021/22 to 2023/24): points, goals scored and conceded, and win rate per match. It is a descriptive before-and-after comparison, not a test of what caused the change.

### 2. Dataset
* **Primary:** La Liga match files from football-data.co.uk, 2018/19 to 2023/24, one row per match (228 Barcelona matches across the six seasons).
* **Second source for checking:** the DataHub season files for the same seasons. Barcelona's matches are joined across the two sources to confirm the records agree.

### 3. Approach
* **Tools:** R, R Markdown.
* **Techniques:** Season-by-season summaries from match-level data, a cross-source join to verify the records, and comparisons in `ggplot2`.
* **Reproducibility:** Relative paths and a self-contained folder, so the whole analysis knits on any machine.

### 4. Results
| Per match, season average | 3 seasons before | 3 seasons after |
|---|---|---|
| Points | 2.18 | 2.16 |
| Goals scored | 2.29 | 1.90 |
| Goals conceded | 0.98 | 0.90 |
| Win rate | 65.8% | 65.8% |

* **The averages hide the swing.** 2021/22, the first season without Messi, was the low point at 1.92 points per match. 2022/23 (league champions, 0.53 goals conceded per match) and 2023/24 both finished above the pre-departure average.
* **Where it changed:** fewer goals scored, offset by fewer conceded.
* **What it can't show:** six seasons can't separate Messi's exit from everything else that changed at the same time, including coaches, the club's finances, new signings and two COVID-affected seasons. No significance test was run, so none of these differences should be read as statistically significant.

### 5. Key Learnings
The biggest takeaway was the importance of **Project Reproducibility**. I initially struggled with absolute file paths that broke the code on different machines. I solved this with a self-contained folder structure and `list.files()` with relative paths, so the entire analysis can be "knitted" by any user with a single click.
