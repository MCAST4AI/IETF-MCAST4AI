The exponential growth in parameter size and training data for Large Language Models (LLMs) is driving increasing complexity and scale in AI computing. Emerging scenarios require efficient data synchronization across geographically distributed data centers and GPU modules within data centers, involving massive point-to-multipoint transmissions. These are not only typical multicast use cases but also impose higher requirements on network multicast capabilities. Applications such as MoE token distribution and model replication etc. are creating new requirements for multicast in AI computing networks.

 

Please check the agenda of the side meeting in the following: 

0. Welcome & Review  Chairs

1. Multicast Requirements and Gap Analysis in AIDC  ( Kefei Liu, China Mobile)  

Abstract: Multicast is a promising technique for enhancing the efficiency of point-to-multipoint data transmission during large language model training and inference in Artificial Intelligence Data Centers (AIDCs). This talk will analyze key requirements of multicast in AIDCs, as well as gaps between capabilities of existing multicast techniques and these requirements.

2. Multicast Requirements and Challenges in Super-node Applications  (Zezhong Yang, UNIVISTA)

Abstract: In recent years, large language models have advanced rapidly. Their unique traffic characteristics impose significant challenges on conventional network components. Offloading computation to network devices has become a critical requirement for the evolution of supernodes, yet many technical challenges remain in implementation.

3. Group RDMA – Reliable Multicast Transmission (Haibo Wang, Huawei)

Abstract: MPI_Bcast, a key collective in HPC, faces performance bottlenecks in RoCE due to the lack of native reliable multicast. Current solutions force a trade-off between software reliability over UD multicast and non-scalable unicast emulation, sacrificing RDMA's low-latency advantage. We propose Group RDMA over RC, where hosts use unmodified RC queue pairs while an Intelligent Switch Fabric performs hardware-level replication of intercepted unicast packets and aggregates ACKs from all receivers. This approach combines RC's strong reliability with hardware multicast efficiency, reducing source CPU load and latency for scalable AI training workloads.

4. Optimized Use of BIER in AIML Data Centers (Jeffery Zhang, HPE)

Abstract: Multicast is gaining traction in AI Data Centers (AIDC) for efficient large-scale data distribution, particularly in collective operations like All2All and AllReduce. Technologies such as In-Network Compute (INC) can also benefit from offloading flow distribution to the network. BIER is particularly suitable for AIDC due to its ability to handle bursty, short-lived all2all flows without requiring per-flow multicast tree state establishment. This document proposes further optimizations for BIER in AIDC and similar deployments, and updates RFC4604 by introducing an IGMP/MLD extension that enables sources to report receiver information to First Hop Routers. This extension is useful in scenarios where the source is unable to impose BIER encapsulation.

5. Open Discussion

 

To further advance this work, currently we have some relevant drafts, which you can access via the following link :

1)Requirements and Gap Analysis of Multicast in AI Data Centers

(https://datatracker.ietf.org/doc/draft-zhang-rtgwg-multicast-requirements-gaps-aidc/)

2)Multicast Use Cases for Large Language Model Synchronization

(https://datatracker.ietf.org/doc/draft-liu-rtgwg-llmsync-multicast/)

3)Multicast usage in LLM MoE

(https://datatracker.ietf.org/doc/draft-zhang-rtgwg-llmmoe-multicast/)

4)Optimized Use of BIER in AIML Data Centers

(https://datatracker.ietf.org/doc/draft-zzhang-bier-optimized-use-in-aidc/)
