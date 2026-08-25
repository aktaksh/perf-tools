

# perf-tools Linux & HFT Study Plan

## Objective

Master Linux performance engineering from first principles using Brendan Gregg's perf-tools. The goal is not to memorize commands but to understand how Linux behaves internally and how to diagnose production performance issues in low-latency trading (HFT) environments.

## Learning Principles

* Always start with first principles before reading the script.
* Understand the Linux subsystem being observed.
* Explain why the tool exists.
* Study how the script works internally.
* Run the tool and interpret every field of the output.
* Map the findings to real production incidents.
* Relate every lesson to latency, jitter, throughput and determinism.
* Finish each lesson with interview questions and a hands-on exercise.

## Standard Lesson Template

1. Problem statement
2. Linux internals involved
3. Relevant kernel path or syscall
4. How the perf-tools script works
5. Script walkthrough line by line
6. Live example output
7. Interpretation of every column
8. Common production failure scenarios
9. HFT relevance and latency impact
10. Troubleshooting workflow
11. Related Linux commands
12. Interview questions
13. Practical exercise
14. Key takeaways

## Learning Order

### Phase 1 - Process Lifecycle
1. execsnoop
2. opensnoop
3. killsnoop
4. newpid

### Phase 2 - Scheduler & CPU
5. runqlat
6. runqslower
7. runqtime
8. wakeuptime
9. offwaketime
10. cpudist
11. offcputime
12. profile

### Phase 3 - Memory
13. cachestat
14. cachetop
15. memleak
16. slabratetop

### Phase 4 - Storage
17. biosnoop
18. biolatency
19. fileslower
20. ext4slower

### Phase 5 - Networking
21. tcpconnect
22. tcplife
23. tcpretrans
24. tcptop
25. hardirqs
26. softirqs

### Phase 6 - Function Tracing
27. funcslower
28. funclatency

### Phase 7 - Advanced Performance
29. perf stat
30. perf record
31. perf report
32. FlameGraphs
33. CPU affinity
34. NUMA
35. HugePages
36. RSS / RPS / XPS
37. DPDK
38. Solarflare OpenOnload
39. eBPF equivalents
40. End-to-end HFT production troubleshooting

## Expected Outcome

By the end of this study plan I should be able to:

* Diagnose Linux performance bottlenecks confidently.
* Explain Linux internals from first principles.
* Read and understand perf-tools source code.
* Correlate CPU, scheduler, memory, storage and networking behaviour.
* Troubleshoot latency and jitter in production.
* Answer senior Linux and HFT infrastructure interview questions with practical examples.
* Design and tune low-latency Linux platforms for trading systems.