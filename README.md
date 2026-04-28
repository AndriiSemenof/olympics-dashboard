# Olympics-dashboard
Interactive PostgreSQL + Tableau dashboard analyzing Olympic Games data (1960 - 2016): medal efficiency by country, athlete physique trends, and sport statistics.

# Olympics Analytics Dashboard

This project explores historical Olympic Games data through 
an interactive analytics dashboard. The backend is a normalized 
PostgreSQL database with four tables - Athletes, Events, Countries, 
and Athlete_Event - loaded from CSV files. The dashboard visualizes 
medal efficiency rankings by country, a world map of Olympic 
performance, a height/weight scatter plot by sport, and the physical 
evolution of athletes from 1960 to 2016.

## Dashboard
[View on Tableau Public](https://public.tableau.com/views/OlympicAnalysisProject/ChampionsProfileGlobalEfficiencyPhysicalTrends?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Tech Stack
1. PostgreSQL 17
2. Tableau Public

## Database Schema
See `/sql/SOL_olympics_datenbank.sql`

## Setup
1. Run `/sql/SOL_olympics_datenbank.sql` to create the schema
2. Adjust the file paths in the COPY commands to your local system
3. Place your CSV files in the adjusted path and run the import

## Data
CSV files are not included (private course data).



# Olympics Analytics Dashboard

Interactive analytics dashboard exploring Olympic Games data (1960-2016).  
Built with a normalized PostgreSQL database and visualized in Tableau Public.

**[View Live Dashboard on Tableau Public](https://public.tableau.com/app/profile/andrii.semenov/viz/OlympicAnalysisProject/ChampionsProfileGlobalEfficiencyPhysicalTrends)**

---

## Key Findings

**Medal Efficiency Rankings (medals per athlete/participation):**
- 🥇 Russia - efficiency score **0.71** (highest among all nations)
- 🥈 USA - **0.62**
- 🥉 Germany - **0.50**

> Efficiency metric normalizes raw medal counts by participation volume,  
> making it a fairer cross-country comparison than total medals alone.

**Physical Evolution of Athletes (1960-2016):**
- Average athlete height and weight have increased steadily over 56 years
- The trend accelerated after 1990, likely reflecting professionalization  
  and sport-specific physical selection
- Clear positive correlation between height and weight across all sports

**Athlete Physique by Sport:**
- Heavy sports (avg. weight 90–100 kg) cluster at heights 175-178 cm
- Tall sports (avg. height 185–192 cm) are not always the heaviest -  
  suggesting sport-specific body type optimization

---

## Tech Stack

| Tool | Purpose |
|---|---|
| PostgreSQL 17 | Normalized relational database (4 tables) |
| SQL | Data cleaning, aggregation, joins |
| Tableau Public | Interactive dashboard & visualizations |

---

## Database Schema

Normalized schema with 4 tables: `Athletes`, `Events`, `Countries`, `Athlete_Event`

See full schema: `/sql/SOL_olympics_datenbank.sql`

---

## Repository Structure

```
  olympics-dashboard/
  ├── README.md
  ├── LICENSE
  └── sql/  
      └── SOL_olympics_datenbank.sql
```
---

## About 

The dataset was provided as part of a private course curriculum 
and is not publicly available. The database schema and SQL queries 
are fully documented and demonstrate the data modeling approach.

