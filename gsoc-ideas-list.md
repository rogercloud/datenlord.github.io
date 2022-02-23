# Ideas List of DatenLord

## Concurrent Hashmap Bench Framework in Rust
Implement a concurrent hashmap benchmark framework which is used to test performance of a concurrent hashmap in Rust. The framework can test the performance of concurrent hashmap with different parameters.

Main functionalities：
- Different percentages of read, update, delete operations
- Different load factors
- Different numbers of concurrent threads
- Different key/value types

## RCU Library in Rust
Implement a userspace [RCU](https://liburcu.org/) library in Rust.

Prerequisite Knowledge:
- atomic operation
- memory model