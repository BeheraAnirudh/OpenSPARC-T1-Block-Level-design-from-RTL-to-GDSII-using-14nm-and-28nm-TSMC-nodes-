OpenSPARC T1 Physical Design – RTL to GDSII
Technology Nodes: 14nm & 28nm (TSMC)
EDA Tools: Synopsys Design Compiler (DC), IC Compiler II (ICC2)

📌 Overview
This project implements the block-level physical design flow for the OpenSPARC T1 processor core, starting from RTL and delivering a clean GDSII ready for fabrication. The design targeted optimal PPA (Power, Performance, Area) while ensuring sign-off compliance for manufacturability.

🔧 Methodology
Logic Synthesis

RTL synthesis with Design Compiler targeting 14nm & 28nm TSMC libraries.

Generated an optimized netlist for physical implementation.

Floorplanning & Power Delivery

Achieved 75% core utilization.

Performed density sweeps to evaluate congestion and routability.

Defined power grid with robust IR-drop margins.

Placement & Optimization

Timing-driven standard-cell placement.

Cell sizing, buffer insertion, and re-driving to fix DRVs (capacitance & transition).

Clock Tree Synthesis (CTS)

Balanced skew and latency while minimizing power impact.

Routing & Post-Route Optimization

Performed global & detailed routing with detour minimization.

Multi-corner, multi-mode (MCMM) optimization for setup/hold closure.

Sign-off Verification

DRC, LVS, and antenna checks passed.

Final GDSII validated for tape-out readiness.

📊 Key Results
Utilization: 75% core area

Node Coverage: 14nm & 28nm

Violations: 0 DRC, 0 LVS, 0 antenna issues

PPA: Achieved timing closure across multiple corners with balanced trade-offs

🛠 Tools & Technologies
Synopsys Design Compiler (DC) – Logic Synthesis

Synopsys IC Compiler II (ICC2) – Physical Implementation

Sign-off Tools: StarRC (PEX), PrimeTime (STA)

📂 Repository Structure
├── reports/           # STA, utilization, and DRV reports
├── scripts/           # TCL scripts for automation
├── layouts/           # DEF, GDSII, LEF files
├── docs/              # Methodology documentation
└── README.md          # Project documentation
🚀 Learnings & Contributions
Gained hands-on experience with advanced-node physical design flows.

Strengthened understanding of MMMC analysis, PPA trade-offs, and EDA automation.

Built reusable TCL scripts for flow automation and design validation.

