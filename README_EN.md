# security-skills · Chinese Security Skills for AI Agents

[![CI](https://github.com/wdfdsyhb/security-skills/actions/workflows/lint.yml/badge.svg)](https://github.com/wdfdsyhb/security-skills/actions/workflows/lint.yml) [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE) ![ZCode Skill](https://img.shields.io/badge/AI-ZCode_Skill-purple)

> Original Chinese-language security skills for AI agents (ZCode and others): HW/HVV red & blue playbooks and CNVD/CNNVD reporting procedures, distilled from 64+ field sources and 620 bug bounty writeups — restructured, not copied.

## Skill List

### hw-hunter — HW/HVV, Red & Blue Perspectives

A rare HW/HVV-focused skill on GitHub: one card covers both the attack and defense sides.

- **Red team**: HW scoring rules (a submitted vuln alone scores nothing — access and data score), a 12-category attack × blue-team detection cross-reference, the detection-triangle noise-reduction main line, TAC sandbox detection-chain evasion, AV-evasion essentials
- **Blue team**: readiness checklists (asset inventory SOP / weak-password windows / hardening parameter sheets), detection formulas per attack type (Webshell / cryptomining / EternalBlue / compromise), responsibility table of Chinese security product lines (NTI/TSA/IPS/WAF/ESPC/TAC/UTS-TAM), the three-element incident response method, blue-team countermeasures
- **Interview**: the three conditions of the grading logic, high-frequency red/blue questions with answer points, and a topic checklist

### cnvd-cnnvd — Chinese Vulnerability Reporting

The full CNVD/CNNVD/Butian reporting pipeline, including practical details you will not find in official documents:

- **Platforms**: platform landscape and newcomer ordering, CNVD certificate details (the 50M RMB registered-capital threshold, the 10-case 3+7 structure, the no-mixing-white-box-with-black-box discipline), the case-padding workflow
- **Reports**: the five elements, the three-part template, the severity formula, the harm-escalation chain (single low-severity finding → Critical)
- **Compliance**: clause table of the Network Product Security Vulnerability Management Regulation (unpublished vulns must not leave the country / no disclosure during major events), ten behavioral red lines, linkage with Criminal Law Articles 285/286, attribution self-protection

## Why Original

- Existing agent skill libraries (mostly English) cover only generic methodology; the Chinese HW ecosystem and domestic reporting paths are absent
- The blue-team perspective (detection logic → reverse-engineered red-team noise reduction) is nearly blank in skill form
- Domestic platform details (CNVD thresholds / case structure / compliance clauses) live in word of mouth and appear in no public skill library

## Installation

```bash
# ZCode
cp -r hw-hunter cnvd-cnnvd ~/.zcode/skills/
# Other agents with skills support: put the directories into the corresponding skills path
```

Each skill = one `SKILL.md` router (~100 tokens of resident metadata) + `references/` deep-dive files loaded on demand.

## Disclaimer

For security learning and research in authorized environments only. Testing unauthorized systems is illegal in China (Cybersecurity Law; Criminal Law Articles 285/286). Companion tutorial book: [security-handbook](https://github.com/wdfdsyhb/security-handbook) (22 chapters, online).

> 🇨🇳 中文文档: [README.md](README.md)
