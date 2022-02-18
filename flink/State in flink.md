Checkpoint in Flink
=====
## Checkpoint流程简介
1. JM trigger checkpoint
2. Source 执行checkpoint的请求，自己开始做 snapshot，并往下游发送 barrier
3. 下游接收 barrier（需要 barrier 都到齐才会开始做 checkpoint）
4. local
5. remote
6. finish

## Checkpointing under backpressure（https://nightlies.apache.org/flink/flink-docs-master/docs/ops/state/checkpointing_under_backpressure/#checkpointing-under-backpressure）

## Incremental Checkpoints 
#### (https://nightlies.apache.org/flink/flink-docs-master/docs/ops/state/state_backends/#incremental-checkpoints)
#### (https://flink.apache.org/features/2018/01/30/incremental-checkpointing.html?spm=a2csy.flink.0.0.2ac03bdc6nP3dc)
 - RocksDB StateBackend

## Tuning Checkpoints and Large State 
#### (https://nightlies.apache.org/flink/flink-docs-master/docs/ops/state/large_state_tuning/#tuning-checkpoints-and-large-state)

 - 

 ## Forward
 #### (https://flink-learning.org.cn/article/detail/3d7ccd2f4d8800f748859ef6ba1e6b55?tab=suoyou&page=4)