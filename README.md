# qaoa-performance-qokit-jpmc
Performance enhancement of QOKit for JPMorgan Chase Quantum Innovation Challenge

## Overview

Quantum computers offer a potential solution to optimize modern business processes, improving quality, speed, cost, and solution applicability. For instance, in finance, quantum optimization algorithms can find optimal asset or financial instrument sets for maximum returns under risk constraints, known as Portfolio Optimization (PO). QAOA, a leading proposal, combines algorithmic and computational steps, leaving room for further performance improvements.

Your challenge is to enhance QAOA on JPMC’s QOKit, such as speeding up single-core CPU performance, improving scaling strategies for large CPU/GPU clusters, enhancing initial states and/or mixers for portfolio optimization, or other areas.

**Code:** QOKit
**Data:** QOKit Toolkit and Examples
**Watch the Launch Webinar Recording For JPMC Here**

## Challenge Information

### Phase 2 Submission Criteria: Performance Exploration & Benchmarking

In this phase, your objective is to profile and enhance the performance of QOkit when simulating the Quantum Approximate Optimization Algorithm (QAOA). You will identify a system bottleneck, implement a targeted improvement, and generate baseline benchmarks to guide final evaluation in Phase 3.

1.  **Bottleneck Identification & Performance Hypothesis**
    Begin by analyzing QOkit’s internal structure to identify a performance-critical component that limits scalability or efficiency. Possible targets include:
    *   Mixer initialization or gate construction overhead
    *   Matrix exponentiation during Hamiltonian evolution
    *   Angle pre-computation routines
    *   Shot-based sampling inefficiencies
    *   Gradient or cost function evaluation bottlenecks
    Explain how this component limits performance in typical QAOA workflows and hypothesize what improvement (in speed, memory, or parallelism) might be possible.

2.  **Proposed Technical Enhancements**
    Describe the specific changes you will make to the QOkit pipeline. Enhancements may include:
    *   GPU acceleration for linear algebra operations or state vector updates,
    *   Custom mixer design that simplifies or accelerates unitary generation,
    *   Tensor-based backend replacement to reduce overhead in large-scale simulations,
    *   Parallelization strategies such as batch-evaluating QAOA layers or distributing parameters across CPU cores or GPU threads.
    Detail your plan at the algorithmic, codebase, or infrastructure level, and explain how the modification will address the identified bottleneck.

3.  **Benchmark Design & Baseline Testing**
    Design a reproducible test scenario for evaluating performance before and after your enhancement. Run baseline tests on unmodified QOkit and collect performance metrics. Document your setup and test parameters thoroughly to allow Phase 3 comparison.

4.  **Application Context**
    Briefly contextualize your performance effort by selecting a real-world quantum optimization use case, such as:
    *   Financial portfolio optimization,
    *   Supply chain network design,
    *   Logistics or route optimization.
    This adds practical motivation for why runtime improvements or resource scaling matter and provides a concrete context for interpreting benchmark impact.

5.  **Execution Environment & Resource Plan**
    Please consider which quantum hardware or simulators best align with your proposed solution. Available platforms include:
    *   Amazon Braket SV1, DM1 TN1
    *   Fire Opal error mitigation software + IBM hardware
    *   IBM Eagle r3, Heron r1, Heron r2
    *   IonQ, Aria-1 Forte-1
    *   IQM Garnett
    *   NVIDIA GPUs with Qiskit GPU / Cirq GPU / Pennylane Lightning / Cu Quantum available out of the box.
    *   qBraid QIR simulator
    *   QuEra Aquila
    *   Rigetti Ankaa-2, Aspen M3
    Justify your platform selection(s) and include technical details, such as expected, and provide more details in the next section. Estimate the runtime gains or efficiency improvements you expect based on your modifications and configuration.

### Phase 3: Optimization Depth & Usability Gains

In this final phase, your team will demonstrate the real-world impact of your enhancements to the QOkit simulator. You are expected to validate your performance improvements through full QAOA executions, document practical benefits for research and development, and share reproducible benchmarking artifacts. More details to come for teams downselected to the final in Phase 3. Refer to the FAQs in the Event Overview for more information about team formation, submission, and more.

## Submission Requirements

Maximum 3 pages PDF (not including references), using 11-point Times New Roman font and single spacing, and submit it through the Aqora platform. Only one submission is required per team.

Your submission must attempt to include:
*   Identified the bottleneck and rationale
*   Technical enhancement plan
*   Benchmark test design and baseline results
*   Optimization use case for context
*   Resource estimates and execution strategy for Phase 3

## References

*   Download JPMorgan Chase & Co. Challenge Document: [JPMC - Challenge.pdf]
