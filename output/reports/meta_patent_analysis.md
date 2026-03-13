# Meta Microkernel Patent Analysis

*Generated 2026-03-11 -- Task 1.8*

## Executive Summary

This report analyses 2 Meta patents potentially related to microkernel and operating system architecture, with specific focus on relevance to Horizon OS.

## Target Patents

### US20210286628A1

- **URL:** [US20210286628A1](https://patents.google.com/patent/US20210286628A1/en)
- **Title:** Operating System With A Single Kernel Stack Per Processor
- **Type:** published_application
- **Status:** abandoned
- **Inventors:** Christoph Klee, Bernhard Poess, Facebook Technologies LLC
- **Filing date:** 2021-05-04
- **Number of claims:** 38
- **Classifications:** G06F9/00, G06F9/06, G06F9/44, G06F9/4401, G06F9/4406, G06F9/46, G06F9/48, G06F9/4806, G06F9/4843, G06F9/4881

**Abstract:**

> In one embodiment, a method includes storing thread state information associated with the first user-mode thread into a memory space associated with the first user-mode thread when executing in kernel space in response to a first system call by a first-user mode thread, executing first operations corresponding to the first system call on a processor, where data associated with executing the first operations are stored on a kernel stack associated with the processor, determining to pause the execution of the first operations, enqueuing a workload on a schedule queue for resuming execution of the first operations in a future, where the workload comprises data associated with executing a remainder of the first operations, and executing second operations corresponding to a second system call from a second user-mode thread on the processor, where data associated with executing the second operations are stored on the kernel stack associated with the processor.

**Horizon OS Relevance:** low

Matching keywords (2): operating system, kernel

**Related patents referenced:** US2021286628A1, US11029968B1, US20240095109A1, US12332789B2, US11474861B1, US20050050553A1, US8209704B1, US8359603B1, US20140137183A1, US20150324224A1

---

### US11119931B1

- **URL:** [US11119931B1](https://patents.google.com/patent/US11119931B1/en)
- **Title:** Data pipeline for microkernel operating system
- **Type:** granted_patent
- **Status:** expired
- **Inventors:** Christoph Klee, Bernhard Poess, Facebook Technologies LLC
- **Filing date:** 2019-09-18
- **Number of claims:** 85
- **Classifications:** G06F12/00, G06F12/02, G06F12/08, G06F12/0802, G06F12/0844, G06F12/0855, G06F9/00, G06F9/06, G06F9/46, G06F9/54

**Abstract:**

> In one embodiment, a method includes receiving a request to create a data pipeline by an operating system executing on a computing device. The operating system allocates a shared virtual memory region for the data pipeline. The shared virtual memory region is mapped to a first virtual address space of a first process and a second virtual address space of a second process. The mapping enables the first process and the second process to share data through the shared virtual memory region. Membership information associated with the data pipeline is updated to include the first process and the second process. An access request for accessing the shared virtual memory region is received from the first process, and the access request is granted or denied based on one or more protection policies.

**Horizon OS Relevance:** medium

Matching keywords (3): microkernel, operating system, kernel

**Related patents referenced:** US20110286463A1, US20130246714A1, US20140317380A1, US20150046661A1, US20150347302A1, US20170115923A1, US20180239617A1, US20190073316A1, US20190227804A1, US20200242043A1

---

## Architectural Relevance Analysis

### Connection to Horizon OS

Meta's Horizon OS is the operating system powering the Quest line of VR/MR headsets. The system is understood to use a microkernel-based architecture with hardware isolation, secure enclaves for DRM, and a capability-based security model.

These patents may protect key architectural decisions in Horizon OS, including:

- **Process isolation:** Microkernel designs that isolate applications from the system runtime
- **Hardware abstraction:** Driver isolation techniques for XR-specific sensors (eye tracking, hand tracking)
- **Security domains:** Trusted execution environments for DRM content and user data protection
- **IPC mechanisms:** Efficient message-passing between isolated components (critical for low-latency XR rendering)

### Patent Strategy Implications

If these patents cover fundamental microkernel architecture techniques used in Horizon OS, they may:

1. **Prevent competing XR OSes** from implementing similar isolation architectures without licensing
2. **Create barriers** for open-source XR operating systems that need similar security properties
3. **Protect Meta's moat** in the XR hardware ecosystem by making it difficult to build compatible runtimes
4. **Influence standards** by patenting techniques that become necessary for XR OS implementations

## Methodology

Patent pages were fetched from Google Patents and parsed for metadata. Horizon OS relevance was assessed by keyword matching against 27 architecture-related terms. Related patents were found through both in-page references and Google Patents search queries.

### Limitations

- Google Patents HTML structure may change, affecting parsing accuracy
- Keyword-based relevance analysis is approximate; full claim analysis requires patent attorney review
- Search coverage depends on Google Patents indexing and query design
- Patent status may change between analysis runs
