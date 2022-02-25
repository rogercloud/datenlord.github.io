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


## Epaxos Chaos Engineering Framework in Rust
Epaxos consensus protocol keeps cluster consistency even when some nodes fails. And Chaos Engineering test is one of the best practice to verify the correctness of the protocol implementation. We've implemented this protocol in Rust, so of source we need an Chaos Engineering framework.

Expected Outcomes:
- A framework that can trigger and monitor result of Chaos tests.
- The framework can help reproduce the result if any error met during the tests.

Prerequisite Knowledge:
- Familiar with Rust language
- Epaxos (or Paxos/Raft) consensus protocol 
- Understand Chaos Engineering concept

Possible Mentor:
Jicheng Shi (jicheng.shi@datenlord.io)

Expected Size of the Project:
350 hours

Difficulty Rating:
Hard


## Rust RPC library on RDMA network
RDMA network is widely adopted in date centers for high performance network applications, and RPC is one of most used ways in the network communication. We've published a Rust RDMA lib, based on which a RPC lib is our next step. We can leverage this RPC library in the DatenLord cluster communication.

Expected Outcomes:
- A Rust RPC library

Prerequisite Knowledge:
- Familiar with Rust language
- Familiar with RDMA concept, familiar with RDMA lib is better
- Familiar with famous RPC libs, such as GPRC.

Possible Mentor:
Jicheng Shi (jicheng.shi@datenlord.io)

Expected Size of the Project:
175 hours

Difficulty Rating:
Medium


## Reimplement FUSE using eBPF and Rust
Filesytem in User-SpacE (FUSE) is a Linux kernel module which provides interface to implement user-space filesystem.
However, FUSE has a lot performance penalty due to memory copy when transfering data from user-space to kernel-space.
This idea is to reimplement FUSE using eBPF and Rust, which is to avoid memory copy between user-space and kernel-space data transfer, so as to achieve high-performance.

Expected Outcomes:
- The eBPF implementation of FUSE which avoids memory copy between user-space and kernel-space data transfer.
- The performance evaluation of the eBPF implementation of FUSE.

Prerequisite Knowledge:
- Familiar with eBPF
- Familiar with FUSE library
- Familiar with Rust language
- Familiar with Linux kernel programming

Possible Mentor:
Pu Wang (pu.wang@datenlord.io)

Expected Size of the Project:
350 hours

Difficulty Rating:
Hard


## RDMA kernel module in Rust
Remote Direct Memory Access (RDMA) is a high performance network protocol, widely used in High Performance Computing (HPC).
Currently RDMA has a kernel module written in C, which serves as the bridge between RDMA user-space applications and Linux kernel, that
when RDMA user-space applications invoke certain RDMA API calls, the RDMA kernel module will ask Linux kernel or
the lower level RDMA hardware drivers to performe certain actions, in response to the RDMA API calls.

As Rust is adopted by the Linux kernel community, the very first application of Rust to Linux kernel is to implement harware drivers.
This idea is to implement the RDMA kernel module in Rust, which will benefit RDMA community that provides a safer and easier to maintain RDMA kernel module.

Expected Outcomes:
- The RDMA kernel module implementation in Rust.

Prerequisite Knowledge:
- Familiar with RDMA programming
- Familiar with Rust language
- Familiar with Linux kernel programming

Possible Mentor:
Pu Wang (pu.wang@datenlord.io)

Expected Size of the Project:
350 hours

Difficulty Rating:
Hard


## eBPF hardware accelerator using SpinalHDL
eBPF is a very convenient way to extend Linux kernel, and currently eBPF is widely used in network, security, tracing, etc.
eBPF has a sandbox running in Linux kernel, and eBPF programs run in the sandbox, so as to protect Linux kernel from malicious eBPF programs.
SpinalHDL is a new kind of Hardware Description Language (HDL) based on Scala, which provides a much efficient way for hardware implemention.
This idea is to implement an eBPF accelerator using SpinalHDL, which can directly run eBPF programs on hardware, instead of the sandbox.
The eBPF hardware implementation should be tested using FPGA.

Expected Outcomes:
- The eBPF hardware implementation.
- The performance evaluation of the eBPF hardware implementation.

Prerequisite Knowledge:
- Familiar with Scala and SpinalHDL
- Familiar with eBPF
- Familiar with FPGA programming

Possible Mentor:
Pu Wang (pu.wang@datenlord.io)

Expected Size of the Project:
350 hours

Difficulty Rating:
Hard


## RDMA hardware implementation using SpinalHDL
Remote Direct Memory Access (RDMA) is a high performance network protocol, widely used in High Performance Computing (HPC).
Currently, there is no high-quality open-source RDMA hardware implementation.
SpinalHDL is a new kind of Hardware Description Language (HDL) based on Scala, which provides a much efficient way for hardware implemention.
This idea is to implement RDMA protocol using SpinalHDL and verify the implementation using FPGA. 

Expected Outcomes:
- The RDMA hardware implementation using SpinalHDL.
- The performance evaluation of the RDMA hardware implementation.

Prerequisite Knowledge:
- Familiar with Scala and SpinalHDL
- Familiar with RDMA protocal
- Familiar with FPGA programming

Possible Mentor:
Pu Wang (pu.wang@datenlord.io)

Expected Size of the Project:
350 hours

Difficulty Rating:
Hard
