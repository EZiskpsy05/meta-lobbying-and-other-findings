# eBPF Ecosystem Influence Analysis

*Generated 2026-03-11*

## Summary

- **BPF-related MAINTAINERS sections:** 0
- **Total BPF maintainers/reviewers:** 0
- **Meta-affiliated:** 0 (0.0%)

## BPF Subsystem Sections

| Section | Maintainers | Meta? | Status |
|---------|-------------|-------|--------|

## Known Meta BPF Personnel

| Name | Role | Significance |
|------|------|-------------|
| Alexei Starovoitov | BPF co-maintainer and original author | Co-created eBPF (extended BPF) while at PLUMgrid, then joined Facebook/Meta. Serves as BPF subsystem... |
| Andrii Nakryiko | BPF libraries maintainer, libbpf author | Primary author and maintainer of libbpf, the canonical BPF user-space library. Designed BPF CO-RE (C... |
| Martin KaFai Lau | BPF networking maintainer | Maintains BPF networking components. Contributed BPF socket storage, cgroup BPF, and other networkin... |
| Song Liu | BPF contributor, live patching | Contributed BPF trampoline and live-patching support. Works on BPF performance features used in Meta... |
| Yonghong Song | BPF compiler/BTF contributor | Key contributor to BTF (BPF Type Format) and BPF CO-RE compiler support in LLVM/Clang. Enables the '... |

## Meta Personnel Found in MAINTAINERS

## libbpf Contributor Analysis

- **Total contributors:** 249
- **Total contributions:** 2446
- **Identified Meta contributions:** 1178 (48.2%)

### Top 10 Contributors

| Rank | GitHub Login | Contributions |
|------|-------------|--------------|
| 1 | anakryiko | 1178 |
| 2 | yonghong-song | 71 |
| 3 | d-e-s-o | 61 |
| 4 | iii-i | 53 |
| 5 | olsajiri | 43 |
| 6 | borkmann | 42 |
| 7 | tohojo | 40 |
| 8 | alan-maguire | 34 |
| 9 | qmonnet | 32 |
| 10 | kkdwvd | 32 |

## BPF CO-RE Architecture Assessment

**BPF CO-RE (Compile Once, Run Everywhere)**

BPF CO-RE allows BPF programs to be compiled once and run across different kernel versions without recompilation. It relies on BTF (BPF Type Format) metadata embedded in the kernel and libbpf's relocation mechanism.

### Meta Advantage

Meta operates one of the largest BPF deployments in the world, running BPF programs across millions of servers with varying kernel versions. BPF CO-RE was designed to solve Meta's specific problem of deploying BPF programs fleet-wide without per-kernel recompilation. While this benefits all BPF users, the architecture decisions were driven by Meta's scale requirements.

### Design Decisions Favouring Meta Infrastructure

- BTF generation integrated into kernel build (reduces Meta's build burden)
- libbpf as the canonical user-space library (Meta controls the reference implementation)
- CO-RE relocation design optimized for large heterogeneous fleets
- BPF skeleton code generation (bpftool gen skeleton) -- reduces boilerplate for Meta's use cases
- Ring buffer design (bpf_ringbuf) optimized for Meta's tracing workloads

### Community Benefit

BPF CO-RE is genuinely useful for the broader community. However, Meta's control over libbpf and the CO-RE toolchain means that alternative approaches (e.g. BCC's runtime compilation) receive less upstream investment.
