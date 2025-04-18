Non-relational databases

---

# **NoSQL Database**
[[NoSQL]]  is a type of database that provides a mechanism for storage and retrieval of data that is modeled differently from the traditional relational [[SQL]] [[Database]]. They doesn't use tablees with fixed rows and columns, even require a fixed schema, they can handle increasead load by adding more servers designed to run on clusters.

# **Types of NoSQL Databases:**
We have:

1. **[[Document Stores]]** ([[MongoDB]], [[CouchDB]]):
    
    - Store data in documents (typically JSON/BSON)
        
    - Good for content management, catalogs, user profiles
        
2. **[[Key-Value Stores]]** ([[Redis]], [[DynamoDB]]):
    
    - Simple pairs of keys and values
        
    - Great for caching, session management
        
3. **[[Column-Family Stores]]** ([[Apache Cassandra]], [[HBase]]):
    
    - Store data in columns rather than rows
        
    - Excellent for analytics and large datasets
        
4. **[[Graph Databases]]** ([[Neo4j]], [[ArangoDB]]):
    
    - Store data in nodes and relationships
        
    - Perfect for social networks, recommendation engines