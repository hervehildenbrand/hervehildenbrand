# Hervé Hildenbrand

**Network Engineering Manager | Architecting Resilient Backbone and Datacenter Solutions | Team Leadership & Technical Excellence**

Building resilient, automated backbone networks at scale. 25+ years designing Internet edge architectures, EVPN/VXLAN data center fabrics, and Segment Routing infrastructures. Creator of open-source network observability tools adopted by the community.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://www.linkedin.com/in/hervehildenbrand/) [![Email](https://img.shields.io/badge/Email-Contact-red)](mailto:herve.hildenbrand@gmail.com)

---

## 🔧 Core Expertise

- **Backbone & WAN Architecture:** SR-MPLS, TI-LFA, BGP PIC, LDP-to-SR migrations, Route Reflector design
- **Data Center Fabrics:** EVPN/VXLAN, MLAG, Arista EOS, Juniper MX/QFX
- **DDoS Defense & Ingress Architecture:** BGP Flowspec, Anycast CDN, WAF-first ingress, scrubbing orchestration
- **Network Automation:** Python, Ansible, Terraform, ANTA framework, API-first design
- **AI-Assisted Operations:** Claude Code, GAIT methodology, autonomous config generation
- **Physical Layer & Resilience:** Fiber diversity auditing, KMZ validation, Tri-Homing, OOB design

---

## 🚀 Open Source Tools

### [gtrace](https://github.com/hervehildenbrand/gtrace) — Advanced Network Path Analysis
```
⭐ 32 stars · 7 forks · Go · MIT License
```
Next-generation traceroute tool with MPLS/ECMP detection, GlobalPing integration, and MTR mode. Performs real-time path analysis across global vantage points, identifies MPLS label stacks, detects per-flow load balancing, and maps autonomous system boundaries. Integrated into [NetClaw by automateyournetwork](https://github.com/automateyournetwork) for third-party network automation workflows.

**Key Features:** MPLS label stack decoding, ECMP path enumeration, GlobalPing distributed tracing, MTR continuous mode, ASN mapping, GeoIP enrichment

### [bgp-explorer](https://github.com/hervehildenbrand/bgp-explorer) — AI-Powered BGP Analysis
```
⭐ 22 stars · 5 forks · Python · MIT License
```
AI-powered CLI and MCP server for querying live and historical Internet routing data. Combines RIPE RIS, RouteViews, RPKI validation, and IRR data into a unified interface. Built for network engineers who need instant BGP visibility without juggling multiple looking glasses. Powers real-time prefix monitoring, AS relationship analysis, and ROA/RPKI compliance auditing.

**Key Features:** Live BGP table queries, RPKI/ROA validation, AS path analysis, prefix hijack detection, historical routing data, MCP server integration for AI agents

### [kentik-mcp](https://github.com/hervehildenbrand/kentik-mcp) — Kentik Observability MCP Server
```
⭐ 2 stars · Go · MIT License
```
MCP server exposing Kentik network observability to AI agents — 8 tools covering flow queries, DDoS alerting, BGP routing, synthetic monitoring, and AI-powered traffic analysis. Enables autonomous network investigation workflows where AI agents query production telemetry directly.

### [ralph-red-vs-blue-v4](https://github.com/hervehildenbrand/ralph-red-vs-blue-v4) — Chaos Engineering for Networks
CCIE+ Expert-Level Chaos Engineering Challenge using RALPH + GAIT methodology. Red team injects realistic network failures; blue team uses AI-assisted agents to detect, diagnose, and remediate — all tracked through git-based audit trails.

### [bgp-radar](https://github.com/hervehildenbrand/bgp-radar) — BGP Monitoring Dashboard
Real-time BGP prefix monitoring and anomaly detection tool built in Go.

---

## 🎤 Speaking & Community

- **LinkedIn Technical Writing** — 17 deep-dive articles reaching 3,200+ followers in 4 months, covering backbone design, BGP optimization, DDoS defense, and engineering leadership
- **Open Source Adoption** — gtrace integrated into third-party automation platforms; bgp-explorer used by network operations teams globally

---

## 📚 Technical Articles & Deep Dives

### Backbone Architecture & BGP Design

#### [Stop Designing Route Reflectors Like It's 2005 (Part 1: The Structural Brain)](https://www.linkedin.com/pulse/stop-designing-route-reflectors-like-its-2005-part-1-hildenbrand-3eope)
*April 2, 2026*

Introduces "Org-Chart Architecture"—a networking twist on Conway's Law where your topology mirrors your team silos. Argues that route reflection is a pure compute problem, not a forwarding problem. Covers the x86 vRR vs hardware RR trade-off, the Out-Of-Path mandate, structural obscurity using RFC 1918 addressing, and the Traffic Gravity trap that can vaporize an RR during a fiber cut.

**Key Topics:** Route Reflector design, Org-Chart Architecture, x86 vRR, Out-Of-Path RR, CoPP limitations, IS-IS overload bit, BGP control plane isolation

---

#### [The Overclock Illusion: Why Aggressive IGP Tuning is Killing Your Network](https://www.linkedin.com/pulse/overclock-illusion-why-aggressive-igp-tuning-killing-your-herve-kmfvf)
*March 13, 2026*

Debunks the practice of reducing IGP hello/dead timers for faster convergence. Explains why protocols already react instantly to direct interface failures via hardware interrupts, and why overclocking creates control plane starvation, transient micro-loops, and broken SSO failovers. Introduces the "Decoupled Speed Framework": BFD for detection, adaptive throttling, TI-LFA for protection, and BGP PIC for overlay convergence.

**Key Topics:** IGP timer tuning, BFD, control plane starvation, micro-loops, SSO breakage, TI-LFA, BGP PIC Core/Edge, convergence architecture

---

### Physical Layer & Infrastructure Resilience

#### [The Backhoe Checkmate: Why Dual Homing is a Scheduled Outage](https://www.linkedin.com/pulse/backhoe-checkmate-why-dual-homing-scheduled-outage-herve-hildenbrand-gambf)
*March 12, 2026*

Argues that 1+1 fiber protection is negligent for mission-critical DCI. Exposes Shared Risk Link Groups hiding in "diverse" paths and the "Silent Reroute" where carriers secretly consolidate your circuits. Introduces the Tri-Homing standard as the minimum viable architecture, driven by database quorum requirements to prevent split-brain catastrophes. Proposes satellite and internet tunnels as the "lifeline" third path.

**Key Topics:** Tri-Homing, SRLG, dual-homing failure modes, split-brain prevention, database quorum, Starlink/LTE backup, KMZ audit

---

#### [Paper Diversity: Why Your IGP Redundancy is a Layer 1 Lie](https://www.linkedin.com/pulse/paper-diversity-why-your-igp-redundancy-layer-1-lie-herve-hildenbrand-ivzoe)
*March 4, 2026*

Exposes how logical redundancy at the routing layer masks physical singularity. Explains the IRU Shell Game (competing carriers sharing trenches), the DWDM Illusion (protected WDM in shared conduits), and the three deadly pinch points: bridge attachments, last 100 feet, and single Meet-Me Rooms. Mandates KMZ-based geospatial auditing and explains why carriers fight to hide their route data.

**Key Topics:** Paper diversity, IRU agreements, DWDM illusion, KMZ geospatial audit, fiber pinch points, MPOE diversity, carrier security theater

---

#### [Excavators: The Apex Predator of IT Infrastructure](https://www.linkedin.com/pulse/excavators-apex-predator-infrastructure-herve-hildenbrand-mba4e)
*December 9, 2025*

Building Out-of-Band management networks that survive when production dies. Introduces the "Ghost Network Principle" and "Cosmetic OOB" anti-pattern. Covers the hybrid reality of "paving the desire path" (use in-band daily, keep OOB for crisis), IPsec hub-and-spoke architecture over regular internet, cellular as the ultimate air-gap, console server strategy, and the discipline of verifying OOB connectivity before every risky change.

**Key Topics:** Out-of-Band management, OOB network design, Ghost Network principle, IPsec VPN architecture, cellular backup, console servers, disaster recovery, pre-flight verification discipline

---

### Enterprise Internet, DDoS Defense & Ingress Architecture

#### [The Enterprise-as-a-CDN: Mastering Anycast Ingress from the Trenches](https://www.linkedin.com/pulse/enterprise-as-a-cdn-mastering-anycast-ingress-from-herve-hildenbrand-mfgte)
*January 29, 2026*

Blueprint for transforming a sovereign backbone into a private Anycast CDN. Load Balancers inject /32 service prefixes into BGP, turning the network into a distributed destination. Covers Traffic Gravity prediction, the Concentration Trap, weaponizing gravity as a "Honeypot" DDoS defense, the /32 scalpel for internal traffic engineering while keeping the external /24 stable, and why BGP PIC is non-negotiable for sub-50ms failover.

**Key Topics:** Anycast CDN architecture, BGP /32 injection, Traffic Gravity engineering, DDoS honeypot strategy, BGP communities automation, BGP PIC, load balancer multiplexing

---

#### [The Great Separation: Why Your Firewall is the Wrong Tool for Ingress](https://www.linkedin.com/pulse/great-separation-why-your-firewall-wrong-tool-ingress-hildenbrand-wkdhe)
*January 20, 2026*

Challenges the "Firewall Everything" orthodoxy. Explains why stateful firewalls become performance suicide pacts for ingress: the State Police problem (conntrack table exhaustion), the Asymmetry Trap (breaking ECMP with stateful devices), and the multiplexing advantage of load balancers. Proposes a decision matrix: Flowspec/ACLs for L3/4, WAF on LB for L7, firewalls reserved strictly for egress C2 prevention.

**Key Topics:** Stateful firewall limitations, ingress architecture, WAF-first design, load balancer multiplexing, ECMP asymmetry, Flowspec L3/4 filtering

---

#### [Building Enterprise Internet Connectivity: A Practical Guide from the Trenches](https://www.linkedin.com/pulse/building-enterprise-internet-connectivity-practical-guide-herve-uwise)
*November 27, 2025*

Blueprint for architecting a sovereign enterprise edge. Covers why your default route is a liability, the "Two-Provider Trap" and diversity audit, why 100G is the new baseline (capacity as a security feature), the Transit/Peering hierarchy, IXP-based cloud connectivity (kill the VPN), Tier-1 myths vs regional advantages, and the BGP Communities "cheat code" for granular traffic engineering.

**Key Topics:** Enterprise BGP architecture, AS autonomy, IXP peering, Tier-1 vs regional providers, BGP communities, traffic engineering, cloud connectivity via IX, Kentik monitoring, network sovereignty

---

#### [DDoS Defense by Design: Architecture That Survives When Everything Else Fails](https://www.linkedin.com/pulse/ddos-defense-design-architecture-survives-when-herve-hildenbrand-q0kre)
*December 2, 2025*

Defense-in-depth strategy born from a real attack. Introduces "Scrubbing Blindness" and the "DEFCON 2 Principle"—pre-configure your reactions, let the network execute autonomously. Covers three-speed detection (Kentik for strategic, Akvorado for tactical, FastNetMon for sub-second reaction), Flowspec as first line defense, why RTBH is "Voluntary Extinction," and the "/32 Trick" for surgical scrubbing using prefix polarization.

**Key Topics:** DDoS mitigation architecture, BGP Flowspec automation, scrubbing center orchestration, FastNetMon, RTBH alternatives, prefix slicing and polarization, detection-to-action automation, DEFCON 2 readiness

---

### Segment Routing & Fast Convergence

#### [The Paranoia Audit: Why I Checked a "Perfect" Network](https://www.linkedin.com/pulse/paranoia-audit-why-i-checked-perfect-network-herve-hildenbrand-gvh4e)
*December 22, 2025*

A practical field guide to verifying sub-50ms convergence actually works. Introduces the "Convergence Triangle" audit covering three layers: Transport (TI-LFA with `weight 0xf000` backup paths), Service (BGP PIC Edge with `weight 0x4000` backups), and the hidden killer—Label Allocation modes. Explains why Per-Prefix allocation breaks PIC and why LOS detection (2-5ms) beats BFD (900ms+) for direct fiber links.

**Key Topics:** BGP PIC Edge, BGP PIC Core, TI-LFA verification, Add-Path configuration, sub-50ms convergence, Juniper MX, FIB weight analysis, label allocation modes, LOS vs BFD detection

---

#### [One IP, Many Ports, Zero Downtime: The BGP Flowspec Story Behind Our Migration](https://www.linkedin.com/pulse/one-ip-many-ports-zero-downtime-bgp-flowspec-story-herve-hildenbrand-ratke)
*December 16, 2025*

Repurposed BGP Flowspec from DDoS defense to surgical traffic migration. Moved hundreds of TCP ports from legacy infrastructure to cloud—port by port—using Flowspec redirection to Anycast anchors over MPLS. Built a three-layer safety architecture: Terraform GitOps interface, CI/CD validation pipeline, and network-side hard filters that reject any unauthorized Flowspec rules. Addresses why Flowspec terrifies engineers and how to cage the "Global Kill Switch."

**Key Topics:** BGP Flowspec traffic engineering, Anycast migration, MPLS label stacking, L3VPN split-brain, Terraform GitOps, Juniper MX204, defense-in-depth automation

---

#### [Segment Routing isn't just "the next fancy protocol"](https://www.linkedin.com/pulse/segment-routing-isnt-just-next-fancy-protocol-herve-hildenbrand-sswte)
*November 23, 2025*

The story of migrating a 50+ circuit European backbone from MPLS/LDP to SR-MPLS—comparing corned beef to wagyu. Reveals the uncomfortable truth: SR migrations succeed or fail based on IGP metric hygiene established years earlier. Covers the transformation from LDP-sync headaches to deterministic Node-SIDs, enabling TI-LFA on every backbone link, and virtualizing the legacy LDP backbone inside the new SR infrastructure using EVPN VPWS.

**Key Topics:** SR-MPLS migration, LDP to Segment Routing, TI-LFA, IS-IS metrics, EVPN VPWS, Node-SID, Juniper SR implementation, IGP foundation design

---

### Network Automation & AI

#### [The "Translation Layer": How I Used AI to Kill My Technical Debt](https://www.linkedin.com/pulse/translation-layer-how-i-used-ai-kill-my-technical-debt-hildenbrand-rsite)
*January 12, 2026*

Migrated legacy Arista Route-Maps to modern Routing Control Functions (RCF) using the Ralph AI agent with zero human intervention. Introduces the GAIT methodology (Git-based Autonomous Iteration with Tracking)—a persistent loop where every AI action is committed to git, enabling safe rollback and auditable automation. The AI learned RCF syntax from Arista documentation, self-corrected errors, and completed the migration in 90 minutes with zero BGP session disruptions.

**Key Topics:** AI network automation, Arista RCF, Route-Map migration, Claude Code, GAIT workflow, Ralph agent, git-based config management, ContainerLab

---

#### [From "Hello World" to "Agent Ready": Why We Built Instead of Bought](https://www.linkedin.com/pulse/from-hello-world-agent-ready-why-we-built-instead-herve-hildenbrand-psite)
*December 30, 2025*

Scaled network validation from 12 tests on a single switch to 288 devices in 121 seconds using ANTA (Arista Network Testing Automation). Built a production-grade API wrapper with contextual validation catalogs (Spines, Leafs, Border Leafs, Storage, OOB) enabling Machine-to-Machine operations. The API-first design prepares infrastructure for autonomous AI agents by turning unpredictable CLI users into predictable API consumers.

**Key Topics:** ANTA framework, network validation at scale, API-first design, contextual testing catalogs, M2M architecture, agentic AI readiness, FabricView dashboard

---

### Network Fundamentals

#### [Why Static Routes Should Be Banned from Production](https://www.linkedin.com/pulse/why-static-routes-should-banned-from-production-herve-hildenbrand-w0h6e)
*February 10, 2026*

A manifesto against hardcoded routing in production networks. Exposes the "Silent Failure" (zombie routes on dead devices), the "Middleman Mask" (L2 switches hiding remote failures), and introduces "HRP" (Human Routing Protocol) as the anti-pattern. Covers why static routes kill automation idempotency, create unauditable technical debt at scale, and why "it's too complicated" is a skills gap problem, not a protocol problem.

**Key Topics:** Static routing anti-patterns, dynamic routing advocacy, BFD limitations with static routes, gray failures, zombie routes, network automation idempotency

---

### Leadership & Engineering Culture

#### [The Cook vs. Chef Paradox: Why the Network Engineer Career Ladder Is Breaking](https://www.linkedin.com/pulse/cook-vs-chef-paradox-why-network-engineer-career-herve-hildenbrand-dyd2e)
*February 18, 2026*

Identifies the structural crisis in network engineering: AI and NetDevOps have automated the "Cook" (execution specialist) out of the kitchen, destroying the proving ground where juniors learned. Argues that survival requires moving from execution to high-stakes validation and reclaiming "culture générale"—the intellectual breadth that makes engineers irreplaceable architects rather than replaceable config translators.

**Key Topics:** Network engineering career crisis, Cook vs Chef analogy, AI impact on networking careers, culture générale, first-principles thinking, validation over execution

---

#### [The Executive Chef's Manifesto: How I Run My Network Kitchen](https://www.linkedin.com/pulse/executive-chefs-manifesto-how-i-run-my-network-herve-hildenbrand-jbnae)
*February 24, 2026*

A leadership framework built on four pillars: Radical Trust (getting in the heat with your team, not hovering), the Learning Tax (demanding the "why" not just the "what"), Ownership Over Speed (infrastructure is a decade-long mission), and the Michelin Pedigree (rewarding performance with complexity, not just compensation). Argues that the best outcome is when your engineers leave to run their own kitchens.

**Key Topics:** Engineering leadership, team management, radical trust, blameless post-mortems, mentorship philosophy, technical leadership culture

---

## 🛠️ Technologies & Tools

```
Routing & Switching   : Juniper MX/QFX, Arista EOS, Cisco IOS-XR
Protocols             : BGP, IS-IS, OSPF, SR-MPLS, EVPN/VXLAN, LDP
Automation            : Python, Ansible, Terraform, Nornir, NAPALM
Validation            : ANTA, pyATS, Batfish
Monitoring            : Kentik, Akvorado, FastNetMon, Prometheus
AI/Agents             : Claude Code, GAIT methodology, Ralph, MCP servers
```

---

## 💡 Current Focus

- **AI-Driven Network Operations:** Building autonomous validation and remediation workflows using GAIT methodology
- **Backbone Architecture:** Route Reflector modernization, BGP PIC optimization, sub-50ms convergence verification
- **Sovereign Ingress:** Anycast CDN architecture, WAF-first design, Traffic Gravity engineering
- **API-First Infrastructure:** Exposing network state as structured JSON for machine consumption and agentic AI
- **Open Source Tooling:** Expanding gtrace and bgp-explorer capabilities for the network engineering community

---

## 🤝 Work With Me

I help enterprises architect resilient backbone networks, modernize BGP infrastructure, and build sovereign ingress architectures that eliminate single points of failure.

**Areas of expertise:**
- Backbone redesign & SR-MPLS migration strategies
- Route Reflector modernization (Org-Chart Architecture)
- DDoS defense architecture & Anycast CDN deployment
- Network automation strategy & AI-assisted operations (GAIT methodology)
- Physical layer diversity auditing & Tri-Homing design

📩 [herve.hildenbrand@gmail.com](mailto:herve.hildenbrand@gmail.com) · [LinkedIn](https://www.linkedin.com/in/hervehildenbrand/)

---

## 📫 Connect

- **LinkedIn:** [linkedin.com/in/hervehildenbrand](https://www.linkedin.com/in/hervehildenbrand/)
- **Email:** herve.hildenbrand@gmail.com
- **GitHub:** You're here — explore the [repositories](https://github.com/hervehildenbrand?tab=repositories)

---

*Network engineering insights from the trenches. All opinions are my own.*
