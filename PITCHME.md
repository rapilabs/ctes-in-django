CTEs in Django?
---------------

 - What is a CTE?  (I stole some slides)
 - Example in SQL and Django
 - Is it useful?
 
https://github.com/rapilabs/ctes-in-django

---

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

The following slides have been lifted from slides 19-69 of 
[Markus Winand's "Modern SQL"](https://www.slideshare.net/MarkusWinand/modern-sql):

---

![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-19-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-20-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-21-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-22-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-23-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-24-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-25-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-26-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-27-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-28-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-29-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-30-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-31-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-32-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-33-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-34-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-35-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-36-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-37-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-38-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-39-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-40-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-41-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-42-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-43-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-44-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-45-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-46-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-47-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-48-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-49-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-50-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-51-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-52-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-53-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-54-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-55-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-56-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-57-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-58-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-59-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-60-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-61-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-62-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-63-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-64-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-65-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-66-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-67-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-68-1024.jpg)
---
![](https://image.slidesharecdn.com/modernsqlinpostgresql-150130134147-conversion-gate01/95/modern-sql-in-open-source-and-commercial-databases-69-1024.jpg)
---


Sample Problem
--------------

from #django IRC channel:

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

```
WITH max_times AS (
  SELECT who, max("when") AS max_when
  FROM activity
  GROUP BY who
)

SELECT * FROM activity a
INNER JOIN max_times m ON m.who = a.who AND m.max_when = a.when
```
http://sqlfiddle.com/#!15/5bc43/2

```
 # assume that Activity's manager is an instance of CTEManager
 max_when = Activity.objects \
     .values('who') \
     .annotate(max_when=Max('when')) \
     .values('who', 'max_when')
 cte = With(max_when)
 cte.join(Activity, who=cte.col.who, when=cte.col.max_when).with_cte(cte)
```

https://repl.it/@rapilabs/django-cte

---

Is it actually useful?

 - Self-joining to an aggregation, but that's solvable by DISTINCT ON (another talk)
 - Readability of SQL is not an issue with ORMs
 - Composability (not with SQL but maybe aide composing w/ ORM api?)
 - Schinckel prefers to write view-backed models that uses subquery in the FROM clause
 - Trees

Limitations:

 - afaik you must have a queryset or model to join the CTE onto
