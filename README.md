# Aggressiveness Index in the Opponent's Half When Losing  

This project leverages **OPTA F24 event data** to develop and analyze a **custom defensive intensity metric**. The goal is to measure how aggressively teams apply pressure in the **opponent's half** when trailing in a match.  

## **Metric: Aggressiveness Index in the Opponent’s Half When Losing**  

### **Definition**  
This metric evaluates the defensive pressure exerted in the **opponent’s half** when a team is losing. It measures the frequency of **tackles, interceptions, ball recoveries, and fouls committed** in this area, divided by the minutes spent behind on the scoreboard.  

### **Formula**  
$$
\frac{\text{Tackles + Interceptions + Ball Recoveries + Fouls Committed in the Opponent’s Half}}{\text{Minutes Losing}}
$$  

### **Filters Applied**  
- Only considers events **when the team is losing**.  
- Field area: **Opponent’s half**.  
- **Included Defensive Actions**:  
  - `7 (Tackle)`, `8 (Interception)`, `49 (Ball Recovery)`.  
  - **Fouls committed**: `4 (Foul)`.  

### **Objective**  
This metric aims to assess how teams react defensively in the **opponent’s half** when trailing, quantifying their high-press intensity.  

By analyzing this metric, we can understand:  
- Whether a team **actively presses to recover possession** and overturn the result.  
- Strategic differences between teams in dealing with adversity.  
- The effectiveness of high-pressure defensive efforts in controlling the game.  

This project applies the metric across all teams in a selected league, contextualizing the results to gain deeper insights into different tactical approaches.

# Results
# Brasileirão
![image](https://github.com/user-attachments/assets/39d638b8-db99-4e32-bcb9-4ae430804d4a)

# Liga Portugal
![image](https://github.com/user-attachments/assets/5de8525b-4e80-4475-9e7b-eba5b6e0e917)

# **Analysis of Defensive Aggressiveness in the Opponent’s Half When Losing**  

The presented graphs illustrate the **defensive aggressiveness** of teams from two different leagues when they are behind on the scoreboard. The calculated value represents the **average number of defensive actions per minute** in the opponent’s half during these periods of disadvantage.  

Each **blue dot** represents a team, while the **dashed red line** indicates the **league average** for this metric, allowing for a direct comparison between teams.  

---  

# **Analysis of the Portuguese League**  
In the first graph, which represents the **Portuguese League**, we observe that:  
- The overall **aggressiveness index** average is **0.52**, meaning that, on average, teams perform **0.52 defensive actions per minute** in the opponent’s half when trailing.  
- **Sporting CP** stands out as the most aggressive team in disadvantage, surpassing all others by a significant margin.  
- Teams like **Benfica and Nacional** also show above-average values, indicating an offensive approach even when behind.  
- On the opposite end, teams such as **Paços de Ferreira, Gil Vicente, and Santa Clara** have significantly lower values, suggesting a more passive or withdrawn posture when losing.  

---  

# **Analysis of the Brazilian League**  
In the second graph, which represents the **Brazilian League**, the key takeaways are:  
- The overall **aggressiveness index** average is **0.49**, slightly lower than in the Portuguese League.  
- **Flamengo** displays an **aggressiveness level far above** other teams.  
- Other teams, such as **Bahia, Coritiba, and Botafogo**, also have values above the league average.  
- On the lower end, teams like **Goiás and Athletico Paranaense** show lower aggressiveness levels, indicating a more cautious approach.  

---  

# **Relevance for Tactical Analysis in Football**  
The metric calculated in this study is highly relevant for **tactical analysis** in football as it contributes to:  

- **Identifying playing styles:** Teams with high values tend to adopt an aggressive, high-pressing mentality, while teams with lower values may follow a more cautious strategy.  
- **Evaluating performance when trailing:** Understanding how a team reacts when losing is crucial for developing comeback strategies or even for controlling an opponent.  
- **Opponent analysis:** Teams can use this data to better prepare against specific opponents, exploiting weaknesses or anticipating behaviors in disadvantageous situations.  

