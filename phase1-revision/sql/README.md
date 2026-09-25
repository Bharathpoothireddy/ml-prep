# SQL Revision

## Goal
Re-activate SQL fundamentals for data science interviews. Focus on 
joins, aggregations, window functions, and CTEs — the four areas 
that show up in almost every SQL round.

## Topics Covered
- INNER / LEFT / RIGHT / SELF joins
- GROUP BY + HAVING
- Window functions: ROW_NUMBER, RANK, DENSE_RANK, SUM() OVER
- CTEs (WITH clauses)
- Subqueries (correlated & non-correlated)
- Date functions
- NULL handling (LEFT JOIN + IS NULL pattern)

## Practice Source
Self-contained schema (customers, orders, products, order_items) 
with 15 problems of increasing difficulty.

## Key Takeaways
- `WHERE` filters rows, `HAVING` filters groups
- `LEFT JOIN + WHERE col IS NULL` = "find missing" pattern
- `RANK` vs `DENSE_RANK` vs `ROW_NUMBER` — know when to use each
- CTEs > nested subqueries for readability
- Window functions ≠ GROUP BY — you keep row-level detail

## Common Interview Pitfalls
- Forgetting `GROUP BY` needs every non-aggregated column
- Using `WHERE` after `GROUP BY` instead of `HAVING`
- Confusing `RANK` (gaps) with `DENSE_RANK` (no gaps)
- Assuming `COUNT(*)` = `COUNT(col)` — the latter skips NULLs
