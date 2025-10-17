---
title: "03 Stlc"
datePublished: Fri Oct 17 2025 04:42:48 GMT+0000 (Coordinated Universal Time)
cuid: cmgud4q5e000102kygcxl3xcw
slug: 03-stlc
tags: shreenibas

---

**STLC (Software Testing Life Cycle)**, its phases, objectives, deliverables, and examples.

---

## **1\. What is STLC?**

**STLC (Software Testing Life Cycle)** is a **sequence of phases** in testing that ensures the **quality of software**. It is part of the SDLC (Software Development Life Cycle) but focuses **only on testing activities**.

**Objective:** To **find defects early**, ensure the software meets requirements, and improve product quality.

**STLC overview** including **Activities, Pre-conditions, Post-conditions, and Deliverables**, and then I’ll provide a **diagrammatic flow**.

---

## **STLC with Activities, Pre & Post Conditions, and Deliverables**

| Phase | Activities | Pre-Conditions | Post-Conditions | Deliverables |
| --- | --- | --- | --- | --- |
| **1\. Requirement Analysis** | \- Review SRS/BRD/FRS  
\- Identify testable requirements  
\- Prepare RTM | SRS / BRD / FRS documents available, stakeholders accessible | Requirements analyzed, RTM created | Requirement Traceability Matrix (RTM) |
| **2\. Test Planning** | \- Define scope of testing  
\- Decide testing types (functional, automation, etc.)  
\- Allocate resources and tools  
\- Estimate effort and schedule | Requirements analyzed, RTM available | Test Plan finalized, resources and strategy assigned | Test Plan Document, Resource Allocation, Test Strategy |
| **3\. Test Case Design / Development** | \- Write test cases based on requirements  
\- Prepare test data  
\- Review test cases | Test Plan ready, requirements analyzed, RTM available | Test Cases and Test Data prepared, RTM updated | Test Cases / Test Scenarios, Test Data, Updated RTM |
| **4\. Test Environment Setup** | \- Setup hardware, software, network  
\- Configure testing tools  
\- Verify environment setup with smoke tests | Test cases and test data ready | Test environment ready for execution | Test Environment Setup Document |
| **5\. Test Execution** | \- Execute test cases manually or via automation  
\- Log defects in tool  
\- Re-test after fixes | Test environment ready, test cases and data available | Test cases executed, defects logged, execution status updated | Test Execution Reports, Defect Logs |
| **6\. Defect Reporting & Tracking** | \- Log defects with severity/priority  
\- Communicate with developers  
\- Re-test resolved defects | Defects identified, defect tracking tool ready | Defects tracked, re-tested, reopened if needed | Defect Reports / Bug Reports |
| **7\. Test Closure** | \- Evaluate exit criteria  
\- Analyze test coverage and metrics  
\- Archive test artifacts  
\- Document lessons learned | All test cases executed, defects resolved or deferred | Test closure completed, metrics analyzed, test artifacts archived | Test Summary Report, Lessons Learned Document |

---

## **STLC Diagram (Flow with Activities, Pre & Post Conditions)**

```java
+-------------------------+
| 1. Requirement Analysis |
| Activities: Review SRS, |
| Identify testable reqs, |
| Prepare RTM             |
| Pre: SRS/BRD/FRS ready  |
| Post: RTM created       |
+-----------+-------------+
            |
            v
+-----------------+
| 2. Test Planning|
| Activities: Define scope, strategy, |
| Allocate resources, Estimate effort |
| Pre: Requirements analyzed           |
| Post: Test Plan ready                |
+-----------+-------------------------+
            |
            v
+-------------------------------+
| 3. Test Case Design / Dev     |
| Activities: Write test cases, |
| Prepare test data, Review      |
| Pre: Test Plan ready           |
| Post: Test cases & data ready |
+-----------+-------------------+
            |
            v
+-----------------------------+
| 4. Test Environment Setup   |
| Activities: Setup env, tools|
| Pre: Test cases & data ready|
| Post: Env ready for testing |
+-----------+-----------------+
            |
            v
+-------------------------+
| 5. Test Execution       |
| Activities: Execute TC, |
| Log defects, Re-test    |
| Pre: Env ready          |
| Post: Execution done    |
+-----------+-------------+
            |
            v
+-----------------------------+
| 6. Defect Reporting & Track |
| Activities: Log & track bugs|
| Pre: Defects found          |
| Post: Defects managed       |
+-----------+-----------------+
            |
            v
+-------------------------+
| 7. Test Closure         |
| Activities: Evaluate,    |
| Archive, Metrics, Lessons|
| Pre: Execution & defects done |
| Post: Closure done       |
+-------------------------+
```

---

✅ **Key Points:**

1. **Activities**: What QA/testers actually do in each phase.
    
2. **Pre-conditions**: What must exist before starting the phase.
    
3. **Post-conditions**: What should be ready after the phase.
    
4. **Deliverables**: The tangible output/document of the phase.