# PostgreSQL Partitioning, JSONB, and Full-Text Search Lab

## 1. Partitioned Posts Table

Created a `posts` table partitioned by `published_at`.

```sql
CREATE TABLE posts (
    id BIGINT GENERATED ALWAYS AS IDENTITY,
    title TEXT NOT NULL,
    body TEXT NOT NULL,
    metadata JSONB DEFAULT '{}',
    search_vec TSVECTOR,
    published_at TIMESTAMPTZ NOT NULL
) PARTITION BY RANGE (published_at);
