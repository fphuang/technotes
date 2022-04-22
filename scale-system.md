Generally, for a read-heavy system, we may consider:
- add more database replicas
- Add caching
- Add elasticSearch / indexing

For a write-heavy system, we may consider:
- Scale up so that we can more concurrent working threads, higher IOPS
- Use NoSQL DB. Then 
  - Scale out and have more shards. Make sure to use consistent hashing and have a carefully chosen sharding key.
  - In case of hot sharding/partitions, try to use auto-resharding (like DynamoDB does)
- Use Distributed DB.
- for very write-heavy small-data system, Redis can be considered.
