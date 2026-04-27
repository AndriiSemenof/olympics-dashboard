# olympics-dashboard
Interactive PostgreSQL + Tableau dashboard analyzing Olympic Games data (1960–2016): medal efficiency by country, athlete physique trends, and sport statistics.

# 🏅 Olympics Analytics Dashboard

This project explores historical Olympic Games data through 
an interactive analytics dashboard. The backend is a normalized 
PostgreSQL database with four tables — Athletes, Events, Countries, 
and Athlete_Event — loaded from CSV files. The dashboard visualizes 
medal efficiency rankings by country, a world map of Olympic 
performance, a height/weight scatter plot by sport, and the physical 
evolution of athletes from 1960 to 2016.

## Dashboard
[View on Tableau Public] (https://public.tableau.com/views/OlympicAnalysisProject/ChampionsProfileGlobalEfficiencyPhysicalTrends?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Tech Stack
- PostgreSQL 17
- Tableau Public

## Database Schema
See `/sql/SOL_olympics_datenbank.sql`

## Setup
1. Run `/sql/SOL_olympics_datenbank.sql` to create the schema
2. Adjust the file paths in the COPY commands to your local system
3. Place your CSV files in the adjusted path and run the import

## Data
CSV files are not included (private course data).
