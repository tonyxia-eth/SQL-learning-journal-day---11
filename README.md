# SQL-learning-journal-day---11

# ⚾ CS50 Moneyball SQL Review – Bite-Sized Testing (Day 11 Night Session)

## ✅ Session Overview

After completing Tasks 1 to 12 of the CS50 Moneyball project, I took time today to slow down and **consolidate my knowledge** through small, focused quizzes and deep self-reflection.

---

## 🧠 Skills Reinforced

- Writing cleaner SQL queries using `AVG()`, `ROUND()`, `SUM()`, `GROUP BY`, and `ORDER BY`
- Understanding when to use **JOINs** and when they're unnecessary
- Learning how to **check database structure** with:
  ```bash
  .tables
  .schema table_name
  SELECT * FROM table_name LIMIT 5;

Debugging errors logically (e.g., checking the correct column name H instead of hits)

Developing habits to explore tables before writing queries

Strengthening understanding of SELECT, aliases (AS), and sorting data effectively

🛠️ Commands Practiced Today

sqlite3 moneyball.db
.tables
.schema performances
SELECT * FROM performances LIMIT 5;
SELECT year, ROUND(AVG(salary), 2) AS "average salary" FROM salaries GROUP BY year ORDER BY year DESC;
SELECT team_id, year, ROUND(AVG(salary), 2) AS "average salary" FROM salaries GROUP BY team_id, year ORDER BY team_id ASC, year DESC;
SELECT year, ROUND(AVG(HR), 2) AS "average home runs" FROM performances GROUP BY year ORDER BY year DESC;
SELECT year, SUM(H) AS "total hits" FROM performances GROUP BY year ORDER BY year DESC LIMIT 5;
🌱 Reflections
Despite working an 8-hour shift and studying late into the night, I maintained my learning momentum.
Tonight wasn't about rushing through new material — it was about deepening my fundamentals through bite-sized tests, real debugging, and building confidence in how to think in SQL.

📅 Status
📖 Day 11 — Night Session Completed

📚 Moneyball Project: Tasks 1–12 fully reviewed

🔥 Ready to push forward into Task 13 and beyond
