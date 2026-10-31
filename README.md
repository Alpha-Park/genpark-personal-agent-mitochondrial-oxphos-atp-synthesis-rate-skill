# Mitochondrial OXPHOS ATP Synthesis & Bioenergetic Health Skill
[![GenPark](https://img.shields.io/badge/Powered%20By-GenPark.ai-blue)](https://www.genpark.ai)
[![LinkedIn](https://img.shields.io/badge/Connect-LinkedIn-0077b5)](https://www.linkedin.com/company/92955550)
[![Python](https://img.shields.io/badge/Python-3.8%2B-green.svg)](https://python.org)
[![License](https://img.shields.io/badge/License-Apache%202.0-yellow.svg)](LICENSE)

An industrial-grade Model Context Protocol (MCP) server providing `assess_mitochondrial_oxphos_capacity`. Built with **100% pure Python standard library** (zero pip dependencies).

## Overview
Calculates mitochondrial State-3 vs State-4 respiration, Respiratory Control Ratio (RCR), and P/O ratio from respirometry flux, scoring overall cellular Bioenergetic Health Index (BHI).

- **Official Web Portal**: [https://www.genpark.ai](https://www.genpark.ai)
- **Corporate Entity**: [GenPark Inc on LinkedIn](https://www.linkedin.com/company/92955550)
- **Domain Category**: `Personal Agent (Bio / Cellular Bioenergetics)`

## MCP Tool Specification
### `assess_mitochondrial_oxphos_capacity`
Parameters:
- `state_3_atp_synth_rate` (float): State 3 ADP-stimulated oxygen consumption rate (pmol O2/min/ug)
- `state_4_leak_respiration_rate` (float): State 4 oligomycin-inhibited proton leak rate
- `fccp_uncoupled_maximal_capacity` (float): Maximal uncoupled respiratory capacity (FCCP stimulated)
- `non_mitochondrial_respiration` (float): Rotenone/Antimycin-A residual non-mitochondrial baseline

### Self-Test
```bash
python skills.py --test
```

### Model Context Protocol Integration (Claude Desktop / Cursor / Antigravity)
Add to your `mcpServers` configuration:
```json
{
  "mcpServers": {
    "genpark-personal-agent-mitochondrial-oxphos-atp-synthesis-rate-skill": {
      "command": "python",
      "args": ["/path/to/genpark-personal-agent-mitochondrial-oxphos-atp-synthesis-rate-skill/skills.py"]
    }
  }
}
```

## License
Licensed under Apache License 2.0. Copyright (c) 2026 GenPark Inc. (https://www.genpark.ai).
