# Hervé Hildenbrand

**Network Engineering Manager | Architecting Resilient Datacenter Solutions | Team Leadership & Technical Excellence**

Building resilient, automated backbone networks at scale. 15+ years designing Internet edge architectures, EVPN/VXLAN data center fabrics, and Segment Routing infrastructures.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/hervehildenbrand/)
[![Email](https://img.shields.io/badge/Email-Contact-red?style=flat&logo=gmail)](mailto:herve.hildenbrand@gmail.com)

---

## 🔧 Core Expertise

- **Backbone & WAN Architecture**: SR-MPLS, TI-LFA, BGP PIC, LDP-to-SR migrations
- **Data Center Fabrics**: EVPN/VXLAN, MLAG, Arista EOS, Juniper MX/QFX
- **DDoS Defense**: BGP Flowspec, RTBH, scrubbing center orchestration
- **Network Automation**: Python, Ansible, Terraform, ANTA framework, API-first design
- **AI-Assisted Operations**: Claude Code, GAIT methodology, autonomous config generation

---

## 📚 Technical Articles & Deep Dives

### Network Automation & AI

#### [The "Translation Layer": How I Used AI to Kill My Technical Debt](https://www.linkedin.com/pulse/translation-layer-how-i-used-ai-kill-my-technical-debt-hildenbrand-oc0pe)
*January 12, 2026*

Migrated legacy Arista Route-Maps to modern Routing Control Functions (RCF) using the Ralph AI agent with zero human intervention. Introduces the **GAIT methodology** (Git-based Autonomous Iteration with Tracking)—a persistent loop where every AI action is committed to git, enabling safe rollback and auditable automation. The AI learned RCF syntax from Arista documentation, self-corrected errors, and completed the migration in 90 minutes with zero BGP session disruptions.

**Key Topics**: AI network automation, Arista RCF, Route-Map migration, Claude Code, GAIT workflow, Ralph agent, git-based config management, ContainerLab

---

#### [From "Hello World" to "Agent Ready": Why We Built Instead of Bought](https://www.linkedin.com/pulse/from-hello-world-agent-ready-why-we-built-instead-herve-hildenbrand-tuyse)
*December 30, 2025*

Scaled network validation from 12 tests on a single switch to 288 devices in 121 seconds using ANTA (Arista Network Testing Automation). Built a production-grade API wrapper with contextual validation catalogs (Spines, Leafs, Border Leafs, Storage, OOB) enabling Machine-to-Machine operations. The API-first design prepares infrastructure for autonomous AI agents by turning unpredictable CLI users into predictable API consumers.

**Key Topics**: ANTA framework, network validation at scale, API-first design, contextual testing catalogs, M2M architecture, agentic AI readiness, FabricView dashboard

---

### Segment Routing & Fast Convergence

#### [The Paranoia Audit: Why I Checked a "Perfect" Network](https://www.linkedin.com/pulse/paranoia-audit-why-i-checked-perfect-network-herve-hildenbrand-hyete)
*December 22, 2025*

A practical field guide to verifying sub-50ms convergence actually works. Introduces the "Convergence Triangle" audit covering three layers: Transport (TI-LFA with `weight 0xf000` backup paths), Service (BGP PIC Edge with `weight 0x4000` backups), and the hidden killer—Label Allocation modes. Explains why Per-Prefix allocation breaks PIC and why LOS detection (2-5ms) beats BFD (900ms+) for direct fiber links.

**Key Topics**: BGP PIC Edge, BGP PIC Core, TI-LFA verification, Add-Path configuration, sub-50ms convergence, Juniper MX, FIB weight analysis, label allocation modes, LOS vs BFD detection

---

#### [One IP, Many Ports, Zero Downtime: The BGP Flowspec Story Behind Our Migration](https://www.linkedin.com/pulse/one-ip-many-ports-zero-downtime-bgp-flowspec-story-our-hildenbrand-wxlhe)
*December 16, 2025*

Repurposed BGP Flowspec from DDoS defense to surgical traffic migration. Moved hundreds of TCP ports from legacy infrastructure to cloud—port by port—using Flowspec redirection to Anycast anchors over MPLS. Built a three-layer safety architecture: Terraform GitOps interface, CI/CD validation pipeline, and network-side hard filters that reject any unauthorized Flowspec rules. Addresses why Flowspec terrifies engineers and how to cage the "Global Kill Switch."

**Key Topics**: BGP Flowspec traffic engineering, Anycast migration, MPLS label stacking, L3VPN split-brain, Terraform GitOps, Juniper MX204, defense-in-depth automation

---

#### [Segment Routing isn't just "the next fancy protocol"](https://www.linkedin.com/pulse/segment-routing-isnt-just-next-fancy-protocol-herve-hildenbrand-gngmf)
*November 23, 2025*

The story of migrating a 50+ circuit European backbone from MPLS/LDP to SR-MPLS—comparing corned beef to wagyu. Reveals the uncomfortable truth: SR migrations succeed or fail based on IGP metric hygiene established years earlier. Covers the transformation from LDP-sync headaches to deterministic Node-SIDs, enabling TI-LFA on every backbone link, and virtualizing the legacy LDP backbone inside the new SR infrastructure using EVPN VPWS.

**Key Topics**: SR-MPLS migration, LDP to Segment Routing, TI-LFA, IS-IS metrics, EVPN VPWS, Node-SID, Juniper SR implementation, IGP foundation design

---

### Enterprise Internet & DDoS Defense

#### [Building Enterprise Internet Connectivity: A Practical Guide from the Trenches](https://www.linkedin.com/pulse/building-enterprise-internet-connectivity-practical-from-hildenbrand-n6flf)
*November 27, 2025*

Blueprint for architecting a sovereign enterprise edge. Covers why your default route is a liability, the "Two-Provider Trap" and diversity audit, why 100G is the new baseline (capacity as a security feature), the Transit/Peering hierarchy, IXP-based cloud connectivity (kill the VPN), Tier-1 myths vs regional advantages, and the BGP Communities "cheat code" for granular traffic engineering.

**Key Topics**: Enterprise BGP architecture, AS autonomy, IXP peering, Tier-1 vs regional providers, BGP communities, traffic engineering, cloud connectivity via IX, Kentik monitoring, network sovereignty

---

#### [DDoS Defense by Design: Architecture That Survives When Everything Else Fails](https://www.linkedin.com/pulse/ddos-defense-design-architecture-survives-when-else-herve-hildenbrand-mfohf)
*December 2, 2025*

Defense-in-depth strategy born from a real attack. Introduces "Scrubbing Blindness" and the "DEFCON 2 Principle"—pre-configure your reactions, let the network execute autonomously. Covers three-speed detection (Kentik for strategic, Akvorado for tactical, FastNetMon for sub-second reaction), Flowspec as first line defense, why RTBH is "Voluntary Extinction," and the "/32 Trick" for surgical scrubbing using prefix polarization.

**Key Topics**: DDoS mitigation architecture, BGP Flowspec automation, scrubbing center orchestration, FastNetMon, RTBH alternatives, prefix slicing and polarization, detection-to-action automation, DEFCON 2 readiness

---

### Infrastructure Resilience

#### [Excavators: The Apex Predator of IT Infrastructure](https://www.linkedin.com/pulse/excavators-apex-predator-infrastructure-build-oob-when-hildenbrand-0hhce)
*December 9, 2025*

Building Out-of-Band management networks that survive when production dies. Introduces the "Ghost Network Principle" and "Cosmetic OOB" anti-pattern. Covers the hybrid reality of "paving the desire path" (use in-band daily, keep OOB for crisis), IPsec hub-and-spoke architecture over regular internet, cellular as the ultimate air-gap, console server strategy, and the discipline of verifying OOB connectivity before every risky change.

**Key Topics**: Out-of-Band management, OOB network design, Ghost Network principle, IPsec VPN architecture, cellular backup, console servers, disaster recovery, pre-flight verification discipline

---

## 🛠️ Technologies & Tools

```
Routing & Switching    : Juniper MX/QFX, Arista EOS, Cisco IOS-XR
Protocols              : BGP, IS-IS, OSPF, SR-MPLS, EVPN/VXLAN, LDP
Automation             : Python, Ansible, Terraform, Nornir, NAPALM
Validation             : ANTA, pyATS, Batfish
Monitoring             : Kentik, Akvorado, FastNetMon, Prometheus
AI/Agents              : Claude Code, GAIT methodology, Ralph, MCP servers
```

---

## 💡 Current Focus

- **AI-Driven Network Operations**: Building autonomous validation and remediation workflows using GAIT methodology
- **SR-MPLS Optimization**: TI-LFA coverage, BGP PIC tuning, sub-50ms convergence verification
- **API-First Infrastructure**: Exposing network state as structured JSON for machine consumption and agentic AI

---

## 📫 Connect

- **LinkedIn**: [linkedin.com/in/hervehildenbrand](https://www.linkedin.com/in/hervehildenbrand/)
- **Email**: herve.hildenbrand@gmail.com

---

<sub>*Network engineering insights from the trenches. All opinions are my own.*</sub>
