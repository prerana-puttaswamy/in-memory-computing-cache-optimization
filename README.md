# Boosting In-Memory Computing: Advanced Cache Optimization Techniques for Hybrid Memory Systems

> Academic Research — Computer Architecture & Systems Design  
> California State University, Long Beach | 2024  
> Author: Prerana Puttaswamy

---

## About

Modern computing systems face a critical bottleneck: processors are fast, but memory access is slow. As datasets grow and applications demand real-time processing, the gap between CPU speed and memory latency — known as the **memory wall** — becomes a key performance limiter.

This research surveys and analyzes **advanced cache optimization strategies** for hybrid memory systems combining DRAM and Non-Volatile Memory (NVM). The goal is to understand how different caching techniques trade off between latency, energy efficiency, and throughput — and which approaches work best under different workload conditions.

---

## Key Research Areas

**Cache Replacement Policies**
- **OptiCache** — optimized cache management that reduces eviction overhead by predicting access patterns
- **MALRU (Modified Adaptive LRU)** — adaptive variant of Least Recently Used that adjusts to workload behavior
- **WADD (Write-Aware Data Displacement)** — write-optimized policy that reduces NVM wear and write amplification

**Memory Architectures**
- Hybrid DRAM/NVM systems — balancing volatile fast memory with persistent slower memory
- Near-Memory Processing (NMP) — moving computation closer to data to reduce data movement overhead
- FPGA-based dataflow cache architectures — hardware-accelerated cache management for high-throughput workloads

**Performance Dimensions Analyzed**
- Access latency across different cache hit/miss scenarios
- Energy consumption per memory operation
- Throughput under read-heavy vs write-heavy workloads
- Scalability under increasing dataset sizes

---

## Key Findings

- Optimized cache replacement policies like OptiCache reduced memory bottlenecks significantly compared to standard LRU under mixed workloads
- Near-memory processing reduced data movement overhead, improving effective throughput for memory-bound applications
- Write-aware policies (WADD) extended NVM lifespan while maintaining competitive read performance
- No single strategy dominates across all metrics — the optimal choice depends on workload type, read/write ratio, and energy constraints
- FPGA-based dataflow architectures showed the highest throughput but at the cost of increased design complexity

---

## Research Paper

The full research paper is included in this repository:

📄 [COA_Research_Paper.pdf](./COA_Research_Paper.pdf)

Topics covered:
- Background on memory hierarchy and the memory wall problem
- Survey of existing cache optimization techniques
- Comparative analysis of hybrid memory architectures
- Performance trade-off evaluation across latency, energy, and throughput
- Recommendations for system designers based on workload characteristics

---

## Concepts & Technologies

| Area | Topics |
|---|---|
| Computer Architecture | Cache hierarchy, memory wall, DRAM/NVM |
| Cache Policies | LRU, OptiCache, MALRU, WADD |
| Processing Paradigms | Near-memory processing, dataflow architecture |
| Hardware | FPGA-based cache management |
| Analysis Dimensions | Latency, energy efficiency, throughput, scalability |

---

## Context

This research was conducted as part of graduate coursework in Computer Architecture at California State University, Long Beach. It contributes to the growing body of work on making hybrid memory systems more efficient for modern data-intensive applications including databases, machine learning inference, and real-time analytics.

---

## Author

**Prerana Puttaswamy**  
MS Computer Science, California State University, Long Beach  
[GitHub](https://github.com/prerana-puttaswamy) | [LinkedIn](https://www.linkedin.com/in/prerana-puttaswamy-a07836224/) | [Portfolio](https://preranap.vercel.app)
