数据库架构设计主要有：shared-Everything , Shared-Disk , Shared-Nothing   
### Shared-Everything
单个主机，完全透明共享CPU/MEMORY/IO，并行能力最差，SMP技术（对称多处理）
### Shared-Disk
处理单元私有CPU/MEMORY，共享磁盘   
Oracle RAC（举例）   
存储器接口达到饱和时候，增加节点不再提升性能
### Shared-Nothing  
处理单元私有CPU/MEMORY/IO，协议通信，并行处理和扩展能力更好(MPP, 大规模并行处理)   
Greenplum、Vertica（举例）     
各个节点处理数据，处理结果向上层汇总或在节点间流转    
