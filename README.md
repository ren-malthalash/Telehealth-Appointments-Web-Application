* Implemented a distributed MySQL setup with primary–secondary failover and region-based write routing so reads and writes stay consistent across nodes.
* Added transaction logging with UUIDs and checkpoints and a recovery flow that replays committed transactions from remote logs after startup.
* Used different isolation levels by operation type and fanned writes to three nodes via Axios for replication.
