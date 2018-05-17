What's a CTE?
-------------

Essentially it's a "temporary view" that only lasts the length of the query:

```
WITH <view-name> AS (
   SELECT *
   … your complex sql…
)

SELECT *
FROM <view-name>
```

---

The following slides have been lifted from lides 19-69 of 
[Markus Winand's "Modern SQL"](https://www.slideshare.net/MarkusWinand/modern-sql):

---

![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-19-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-20-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-21-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-22-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-23-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-24-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-25-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-26-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-27-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-28-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-29-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-30-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-31-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-32-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-33-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-34-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-35-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-36-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-37-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-38-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-39-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-40-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-41-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-42-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-43-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-44-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-45-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-46-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-47-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-48-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-49-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-50-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-51-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-52-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-53-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-54-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-55-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-56-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-57-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-58-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-59-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-60-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-61-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-62-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-63-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-64-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-65-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-66-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-67-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-68-638.jpg?cb=1488960007)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-69-638.jpg?cb=1488960007)
---


Sample Problem
--------------

    If I had a bunch of users with some activity each day, how can I construct a query to get their last activity object on that day for each of the days?

---

Consider the following table:

```
 +—————————————————————————————————————————————————————————————————————————————+
 |                                 Activity                                    |
 +-----------------------------------------------------------------------------|
 |  Who?       |   When?   |    What?                                          |
 +-------------+-----------+---------------------------------------------------|
 |  g1eb       |   9am     |    Go to work                                     |
 |  g1eb       |   5pm     |    Knock-off time!                                |
 |  shangxiao  |   9am     |    Go to work                                     |
 |  shangxiao  |   5pm     |    Knock-off time!                                |
 |  shangxiao  |   6pm     |    Attend MelbDjango                              |
 +-----------------------------------------------------------------------------+
```

We want to know what each person's final activity is:

```
 +-----------------------------------------------------------------------------+
 |  g1eb       |   5pm     |    Knock-off time!                                |
 |  shangxiao  |   6pm     |    Attend MelbDjango                              |
 +-----------------------------------------------------------------------------+
```
---

http://sqlfiddle.com/#!15/5bc43/2

https://repl.it/@rapilabs/django-cte

