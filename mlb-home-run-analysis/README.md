# 🧢 MLB Power Hitter Analysis by Position

This project analyzes historical home run trends in Major League Baseball by player position, debut age, and career length. Using data from the Lahman Baseball Database (1871–2024), the goal is to uncover which positions consistently produce power hitters, and what player archetypes drive long-term success.

While fans and fantasy players often focus on recent stats or name recognition, historical analysis helps surface the roles and traits most likely to generate home run production over time.

---

## 🔍 Key Questions

- Which positions produce the most power hitters historically?
- How do debut age and career length impact HR totals?
- What player archetypes (e.g., early debut + long career) correlate with elite power?
- How have different positions evolved in terms of home run output since 1980?
- How has power output changed over time?

---

## 🛠️ Tools & Techniques Used

- **R** for analysis, visualization, and data cleaning  
- **ggplot2** for static charts and barplots  
- **cowplot** for layout and side-by-side visual comparisons  
- **tidyverse** (`dplyr`, `ggplot2`, `readr`, `tidyr`) for data wrangling and transformation  
- **tidytext** for parsing player position strings  
- **readr** to import raw CSVs from the Lahman dataset  
- **Data joins** across multiple Lahman tables (e.g., `Batting`, `People`, `Fielding`) to create a unified player-position-career dataset  
- **Kaggle** for hosting, writing, and running the analysis notebook

📊 **Visualization types include**:  
Histograms, box plots, scatterplots, bar charts, faceted charts, line charts, and heat maps.
Created **10+ visualizations** to explore debut trends, power output by position, weighted HR averages, career archetypes, and more.

---
## 📊 Featured Visuals

Here are selected visualizations from the analysis that highlight key trends and insights:

### 🔹 Average Home Runs per Season by Position & Decade
This line chart illustrates how offensive output has evolved by position from the 1870s through the 2020s, showcasing league-wide and role-specific shifts in power.
![](MLB%20Visuals/avg_hr_position_decade_linechart.png)

---

### 🔹 Power-Hitter Archetypes by Debut Age & Career Length
This heatmap identifies which player profiles based on debut age and career length tend to deliver the most home runs per year, segmented by position.
![](MLB%20Visuals/player_archetype_grid.png)

---

### 🔹 Average vs. Weighted Home Runs per Season by Position
Side-by-side bar charts compare raw and weighted HR averages. The weighted chart emphasizes the influence of long-tenured sluggers, while the raw chart treats all players equally.
![](MLB%20Visuals/avg_hr_vs_weighted_avg_barcharts.png)

---

### 🔹 HR Distribution by Position (5+ Seasons)
This boxplot displays the interquartile range, median, and outliers for average HRs per season across positions; revealing which roles show consistent power output.
![](MLB%20Visuals/avg_hr_by_position_boxplot.png)

---

### 🔹 Top 5 Power Hitters by Position (Min. 5 Seasons)
A faceted bar chart highlighting the most prolific HR hitters at each position, offering a snapshot of positional ceilings and standouts across eras.
![](MLB%20Visuals/top_5_hitters_by_position_bar.png)

---

## 📁 Dataset Info

- **Source**: Lahman Baseball Database (2025)  
- **License**: [Creative Commons Attribution-ShareAlike 3.0 Unported](http://creativecommons.org/licenses/by-sa/3.0/)  
- **Coverage**: MLB player stats from 1871–2024, including hitting, fielding, and pitching data

---

## ⚠️ Scope & Limitations

- **Pitchers were excluded** from the analysis due to historically negligible offensive contributions. Their removal also reflects modern rule changes—such as the National League adopting the **Designated Hitter (DH)** in 2022—after which pitchers no longer bat.

- **Designated Hitters (DH)** are not included as a standalone position. The Lahman dataset labels DH inconsistently across eras, making it difficult to track as a primary role. Many players served as part-time DHs while still fielding other positions.
  
- **Universal adoption of the DH in the NL (2022)** is a recent structural change that may increase league-wide home run totals going forward. By replacing pitcher at-bats with power-capable hitters, the DH rule expands offensive opportunity. However, there is not yet enough post-2022 data to meaningfully analyze its long-term effect on positional power output. This will be important to monitor in future updates.

- **Shohei Ohtani** does not appear in this analysis. Though a prolific modern power hitter, he is labeled as a **pitcher** in the dataset and was filtered out alongside other pitchers.

- **Home runs per season** were used as a primary metric rather than slugging percentage, wOBA, or plate appearance-adjusted stats. This prioritizes simplicity and visibility in the dataset but may limit comparability between players with uneven playing time.

- **Decade-over-decade comparisons** should be interpreted with caution. MLB rule changes (e.g., 1969 mound lowering), the 1994 strike, changes in drug policy, and the launch-angle revolution all influence offensive environments in ways not directly accounted for in this analysis.

These design choices were made to support **clean, consistent comparisons** across a wide historical range.

---

## 📈 Key Insights

- **Middle infielders** have seen the **largest percentage increase** in HR output since 1980.
- **Early-debuting, long-career** players at traditional slugger roles (e.g., 1B, OF) show the **highest HR rates**.
- **Catchers** remain low-output overall, largely due to shared playing time and defensive emphasis.
- Shorter careers with high HR averages may reflect **peak-power bursts** at more physically demanding positions.
- Historical context matters—league rule changes, equipment updates, and positional evolution all play a role.

---

## 🔮 Looking Ahead

Future enhancements to this project could include:

- Normalizing by **plate appearances** or **slugging percentage**
- Exploring **park factors**, **injury history**, or **handedness**
- Tracking **rule change effects**, like universal DH adoption
- Segmenting further by **league**, **era**, or **archetype groupings**

---

## 📌 Use Cases & Portfolio Value

This project highlights my ability to transform complex, multi-decade sports data into meaningful insights using R and data visualization.

It’s relevant for:

- **Business Intelligence teams** looking to analyze trends over time and communicate findings to non-technical stakeholders.
- **Sports analytics departments** seeking to identify undervalued player archetypes or reassess positional expectations.
- **Fantasy sports platforms** aiming to educate users or improve draft tools based on historical trends.
- **Recruiters and hiring managers** evaluating candidates for data storytelling, visualization, and analytical reasoning skills.

By analyzing over 150 years of MLB hitting data, I showcase how data-driven thinking can uncover strategic insights — whether for front-office decision-making, fan engagement, or product development.

