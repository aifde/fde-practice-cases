# 02. Government of Alberta: AI agents for security review and legacy modernization

English | [中文](README.zh.md) | [日本語](README.ja.md)

| Field | Evidence |
| --- | --- |
| Confidence | High, with results disclosed by the Government of Alberta team through Anthropic |
| Deployment status | In production use since 2025, with continuous review agents added to the development process |
| Customer | Government of Alberta, Ministry of Technology and Innovation |
| AI platform | Claude Code, Claude Opus and Sonnet, and the Claude Agent SDK |
| AI surface | Repository scanning, vulnerability analysis, patch drafting, test generation, modernization, and continuous security review |
| Why it is relevant to AI FDE | A government engineering team adapted frontier coding agents to a large legacy estate, built validation controls, and turned the work into a repeatable operating model |

## Operational problem

Alberta's Ministry of Technology and Innovation supports systems across 27 ministries. The public case describes roughly 1,280 applications and 3,400 code repositories, including older systems that hold tax, procurement, social-services, public-safety, and wildfire-response information. Much of the estate had never received a systematic security review.

The challenge was larger than running a conventional scanner. Older repositories lacked documentation and tests, known-pattern scanners could miss context-dependent risks, and some applications were too outdated to patch efficiently. Any proposed change still had to satisfy public-sector security and release controls.

## Delivery approach

The ministry created an internal team in 2025 to make the estate safer and easier to maintain. The team combined deterministic rules with Claude Code agents. A first stage flagged known patterns. A second stage reviewed those findings in repository context and cited the exact file and line so engineers could verify the result.

When a finding was valid, Claude could draft a patch, write missing tests, and build the change. For systems that were too old to repair safely, the team used the same workflow to understand behavior and support a controlled rewrite. No patch went directly to production. Ministry engineers reviewed and approved it before release.

~~~mermaid
flowchart LR
  A[1,280 applications and 3,400 repositories] --> B[Rules-based scan]
  B --> C[Parallel Claude review agents]
  C --> D[Evidence with file and line references]
  D --> E[Patch and test generation]
  E --> F[Government engineer review]
  F -->|Approved| G[Controlled release]
  F -->|Rejected or revised| C
  G --> H[Continuous red, blue, quality, and accessibility checks]
~~~

## Evaluation and control model

The public design contains several safeguards that are directly relevant to FDE work:

- Findings include repository evidence rather than unsupported prose.
- Tests are created before patching when a codebase lacks adequate coverage.
- Human engineers approve changes before shipment.
- Red-team agents probe an application from the outside, while blue-team agents compare defenses with an international security standard and prepare remediation plans.
- Applications are checked against roughly 95 security controls on each pass.
- Separate agents inspect code quality and public-facing writing.

This is a stronger pattern than asking a coding model to fix a repository autonomously. It separates discovery, evidence, remediation, verification, and release authority.

## Publicly reported outcomes

Anthropic's case study reports that Alberta:

- Assessed 466 million lines of government code in about 20 hours using roughly 50 parallel agents.
- Estimated that an equivalent manual review could have taken about 6.5 years.
- Used agents to find issues missed by traditional automated scanners.
- Generated tests and patches, with engineers reviewing every change before shipment.
- Rebuilt some legacy systems in four to five days when patching was not practical.

These figures are reported by the project participants. Public materials do not provide false-positive rates, severity distribution, independent penetration-test results, or the number of generated patches that were ultimately deployed.

## Why this is a strong AI FDE case

The project started from a concrete operational constraint: a large and sensitive legacy estate that could not be reviewed repository by repository at conventional speed. The team combined AI with deterministic tools, adapted the workflow to government controls, and created reusable agents for continued review. The value came from system design and operating discipline, not from a one-off prompt.

The case reflects an internal forward-deployed pattern. The public material does not say that Anthropic employed a named FDE team on site, so the classification is based on the delivery method rather than a formal job title.

## What remains unproven

- The 6.5-year comparison is an internal estimate, not an observed control-group result.
- The public case does not disclose precision, recall, false-positive rates, or vulnerability-severity counts.
- Security-sensitive details are appropriately withheld, which limits external reproduction.
- Fast code generation does not by itself prove long-term maintainability or lower total cost.

## FDE role alignment

- **R2. Scoping and end-to-end delivery ownership**
- **R3. Hands-on implementation and systems integration**
- **R4. AI workflow and human-control design**
- **R5. Evaluation and production quality**
- **R6. Security, governance, reliability, and cost**
- **R8. Reusable patterns and field feedback**

See the [OpenAI and Amazon FDE role framework](../../role-requirements.md).

## References

1. [Anthropic, Government of Alberta cybersecurity case study](https://www.anthropic.com/news/alberta-government-claude-cybersecurity)
2. [The Velocity White Papers, Government of Alberta technical papers](https://thevelocitywhitepapers.com/)
3. [Government of Alberta, Cybersecurity in Alberta](https://www.alberta.ca/cybersecurity-in-alberta)
