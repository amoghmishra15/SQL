# SQL
## Learning SQL

CREATE TABLE table name (id INTEGER PRIMARY KEY AUTOINCREMENT, name TEXT, quantity INTEGER );

(autoincrement makes it automatically increment, dont need to type it out)
but instead, you'll have to mention the variables where values are being inserted
eg:

---
### INSERT
INSERT INTO table name(type, minutes, calories, heart_rate) VALUES ("biking", 30, 100, 110);

INSERT INTO table name VALUES (1, "Bananas", 4);

---
### AND 
SELECT * FROM exercise_logs WHERE calories > 50 AND minutes < 30;

---
### OR 
SELECT * FROM exercise_logs WHERE calories > 50 OR minutes < 30;

---
### IN
SELECT * FROM exercise_logs WHERE type IN (SELECT type FROM drs_favorites);

### NOT IN
SELECT * FROM exercise_logs WHERE type NOT IN (SELECT type FROM drs_favorites);
