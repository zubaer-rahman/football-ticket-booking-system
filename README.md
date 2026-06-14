# Football Ticket Booking System — PostgreSQL learning Approach

Tiny, focused SQL for practicing PostgreSQL: schema, small sample data, and example queries live in `QUERY.sql`. No app code — just SQL you can read, run, and learn from.

About the script: it uses common Postgres features such as `SERIAL`, `CHECK` constraints, `ILIKE`, `COALESCE`, `JOIN ... USING`, and `LIMIT/OFFSET`.

Quick start
- Create a DB and load the script:

  ```bash
  createdb football_db
  psql -d football_db -f QUERY.sql
  ```

- Run queries with `psql -d football_db`.

- Prefer a GUI client (e.g., Beekeeper Studio or DBeaver) to run the script block-by-block and inspect results interactively — helpful when learning.

Practical tip
- Use explicit transactions for bookings to avoid races. Prefer `SELECT ... FOR UPDATE` when checking availability in concurrent scenarios.

That's it — small, practical, Postgres-first. Open `QUERY.sql` and experiment.

