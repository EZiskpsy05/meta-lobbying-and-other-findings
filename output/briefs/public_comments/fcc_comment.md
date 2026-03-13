# Public Comment -- FCC: Age Verification and Open-Source Impact

*Generated 2026-03-12*

## RE: Connected Device Age Verification -- Open-Source Impact

**Date:** 2026-03-12

**Submitted to:** Federal Communications Commission

**Subject:** Comment on Age Verification Requirements for Connected Devices and Their Impact on Open-Source Firmware and Operating Systems

## Summary of Position

As the Commission considers frameworks for age-appropriate content access on connected devices, we urge consideration of the impact on open-source firmware and operating systems. Many connected devices -- from routers to IoT sensors to educational computers -- run Linux-based software. Mandating device-level age verification infrastructure would effectively require commercial firmware on all consumer connected devices.

## Open-Source in the Connected Device Ecosystem

Open-source software is the backbone of the connected device ecosystem:

- **Routers and networking:** OpenWrt, DD-WRT, and similar Linux-based firmware power millions of consumer routers
- **IoT devices:** Linux runs on the majority of IoT hardware
- **Educational computing:** Raspberry Pi and similar platforms use Linux-based operating systems for STEM education
- **Assistive technology:** Many accessibility devices run open-source software

Mandating device-level age verification would require these devices to integrate with commercial identity services, adding cost, complexity, and privacy concerns.

## Technical Incompatibility

Age verification at the device/OS level assumes:

- A mandatory user account tied to a verified identity
- Network connectivity to a verification service
- A legal entity liable for verification accuracy

Open-source firmware and operating systems are designed to operate without these dependencies. Requiring them would foreclose open-source alternatives for an entire category of consumer electronics.

## Competitive Concerns

We note that vertically integrated platform companies (including Meta Platforms with Horizon OS for VR/AR devices) benefit disproportionately from device-level age verification mandates. These companies already maintain the required identity infrastructure and face negligible compliance costs.

### Research Evidence

- Task horizon-os-audit: Horizon OS has 5 built-in compliance features: Meta Account Age Verification; Get Age Category API; Family Center; Quest
- Task horizon-os-audit: Linux distros have 7 major compliance gaps: Account System Age Bracket; Age Category D-Bus API; Parent-Child Account Lin
- Task 2.1: Meta employees hold 0 maintainer and 0 reviewer positions across 0 kernel subsystems (kernel mainline HEAD). 0 unique in
- Task 2.4: Meta employees hold 0 of 0 BPF maintainer/reviewer positions (0.0%). BPF-related subsystem sections: 0.
- Task 2.4: Alexei Starovoitov: BPF co-maintainer and original author. Co-created eBPF (extended BPF) while at PLUMgrid, then joined
- Task 2.4: Andrii Nakryiko: BPF libraries maintainer, libbpf author. Primary author and maintainer of libbpf, the canonical BPF use
- Task 2.4: Martin KaFai Lau: BPF networking maintainer. Maintains BPF networking components. Contributed BPF socket storage, cgroup
- Task 2.4: Song Liu: BPF contributor, live patching. Contributed BPF trampoline and live-patching support. Works on BPF performance
- Task 2.4: Yonghong Song: BPF compiler/BTF contributor. Key contributor to BTF (BPF Type Format) and BPF CO-RE compiler support in 
- Task 2.7: Licensing pattern identified: 'Restrict-then-Open Cycle'. Meta repeatedly introduces restrictive licensing, faces commun

## Requested Commission Action

We respectfully request that the Commission:

1. **Exempt open-source firmware and operating systems** from device-level age verification requirements
2. **Adopt service-level rather than device-level** verification frameworks that do not discriminate by operating system
3. **Engage the open-source community** in developing any technical standards for connected device safety
4. **Evaluate the competitive impact** of device-level mandates on the open-source hardware/software ecosystem
