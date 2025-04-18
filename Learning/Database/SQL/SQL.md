Relational Databases

---


# **Relational Databases**
[[SQL]] is the standard language for managing **relational databases**, which store data in structured tables with predefined schemas. Unlike [[NoSQL]], SQL databases enforce **[[ACID]] properties** (Atomicity, Consistency, Isolation, Durability) and are optimized for complex queries, transactions, and data integrity.

# **Types of SQL Databases**

1. **[[Row-Oriented Databases]]** ([[PostgreSQL]], [[MySQL]])
    
    - Store data in rows (all columns of a record grouped together)
        
    - Optimized for transactional workloads (OLTP) and complex queries
        
    - Ideal for: ERP systems, e-commerce platforms, traditional CRUD apps
        
2. **[[Column-Oriented Databases]]** ([[Amazon Redshift]], [[Snowflake]]):
    
    - Store data in columns (all values of a field grouped together)
        
    - Optimized for analytical queries (OLAP) and aggregations
        
    - Ideal for: Data warehouses, business intelligence, large-scale analytics
        
3. **[[NewSQL Databases]]** ([[CockroachDB]], [[YugabyteDB]]):
    
    - Combine SQL interfaces with NoSQL-like horizontal scaling
        
    - Maintain ACID compliance across distributed systems
        
    - Ideal for: Globally distributed apps needing strong consistency
        
4. **[[Time-Series SQL Databases]]** ([[TimescaleDB]], [[InfluxDB]]):
    
    - Specialized for timestamped data with time-based partitioning
        
    - Optimized for high-volume metric/event data
        
    - Ideal for: IoT monitoring, financial tick data, observability platforms
        
5. **[[Embedded SQL Databases]]** ([[SQLite]], [[Spring H2]]):
    
    - Serverless, lightweight engines that run in-process
        
    - Single-file storage with zero configuration
        
    - Ideal for: Mobile apps, local caching, edge computing