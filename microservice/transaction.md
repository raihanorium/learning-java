# Microservice Transaction Management

## Challenges of Distributed Transaction
1. **Maintaining ACID:** To ensure the correctness of a transaction, it must be Atomic, Consistent, Isolated and Durable (ACID).
1. **Managing the transaction isolation level:** It specifies the amount of data that is visible in a transaction when the other services access the same data simultaneously.