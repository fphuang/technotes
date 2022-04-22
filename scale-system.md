Generally, for a read-heavy system, we may consider:
- add more database replicas
- Add caching
- Add elasticSearch / indexing
- For NoSQL, consider MongoDB

For a write-heavy system, we may consider:
- Scale up so that we can more concurrent working threads, higher IOPS
- Use NoSQL DB (such as Cassandra). Then 
  - Scale out and have more shards. Make sure to use consistent hashing and have a carefully chosen sharding key.
  - In case of hot sharding/partitions, try to use auto-resharding (like DynamoDB does)
- Use Distributed DB.
- for very write-heavy small-data system, Redis can be considered.


Ref:
1. https://redis.io/docs/getting-started/faq/#:~:text=Redis%20code%20base.-,Can%20you%20use%20Redis%20with%20a%20disk%2Dbased%20database%3F,eventually%20consistent%20on%2Ddisk%20database.
2. 
