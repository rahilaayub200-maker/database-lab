# Database Lab

## MongoDB
- Created a product catalog using MongoDB.
- Inserted products with categories, prices, stock, tags, and ratings.
- Queried Electronics products costing less than $200.
- Used an aggregation pipeline to calculate average ratings by category.

## Redis
- Stored a catalog count using Redis with an expiration time.
- Used a sorted set to organize products by price.
- Used Redis Pub/Sub to publish and receive an inventory update message.

## PostgreSQL and pgvector
- Enabled the pgvector extension in PostgreSQL.
- Created a table containing product embeddings.
- Used vector similarity search to find the two products most similar to a query vector.

## Reflection

This lab helped me understand how different database technologies can work together. MongoDB is useful for flexible document-based product data, while Redis provides fast caching and messaging. PostgreSQL with pgvector can support semantic similarity searches using vector embeddings. Combining these technologies can help build efficient and flexible modern applications.
