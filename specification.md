Prompt Markup Language (PML)
Version: 0.1 – Draft Proposal
Author: Michal Beran, 2025

📄 Purpose of PML
PML is a structured language for defining prompts that allow artificial intelligence to quickly and unambiguously receive the data needed to generate complex outputs, such as:

marketing plans

strategic documents

procedural instructions

medical protocols

any content that benefits from structured logic

The language is inspired by principles of HTML, YAML, and natural language, and is designed specifically for communication with AI.

🛠️ Syntax Variants
1. XML/HTML Style
xml

<Prompt>
  <Goal>Increase sales of car care products</Goal>
  <TargetAudience>
    <Segment>Men aged 25–40</Segment>
    <Segment>Mothers with small children</Segment>
  </TargetAudience>
  <Channels>
    <Channel>Instagram</Channel>
    <Channel>Leaflets at gas stations</Channel>
  </Channels>
  <Message>
    You don’t need time to have a clean car. We’ll do it for you.
  </Message>
  <TimeFrame>Q3 2025</TimeFrame>
  <KPI>
    <Metric>Click-throughs from Instagram</Metric>
    <Metric>Purchases in the e-shop</Metric>
  </KPI>
</Prompt>
2. YAML Style (Recommended for Non-Technical Users)
yaml

Prompt:
  Goal: Increase sales of car care products
  TargetAudience:
    - Men aged 25–40
    - Mothers with small children
  Channels:
    - Instagram
    - Leaflets at gas stations
  Message: You don’t need time to have a clean car. We’ll do it for you.
  TimeFrame: Q3 2025
  KPI:
    - Click-throughs from Instagram
    - Purchases in the e-shop
📘 Usage
Writing Prompts for AI
Instead of free-form text, the user writes prompts in structured PML format. The AI quickly identifies each section.

Managing Marketing Operations
Users can rapidly modify segments, messages, or communication channels.

Integration with Tools (Notion, Zapier, AI engines)
PML can be easily converted to JSON or CSV for integration with automation systems.

📂 Recommended File Extensions
.pml.yaml – for YAML-style syntax while identifying the file as PML

.pml.xml – for XML-style markup syntax

.pml – for use with custom parsers or dedicated environments that natively understand PML

In case of a future “PML browser” that can display, interpret, or render PML files, it's recommended to:

Use .pml as a full-fledged language extension

Retain YAML or XML structure internally for compatibility

Define a MIME type such as application/x-pml for web recognition

This would elevate PML to a self-describing, executable format on par with .html, .json, or .md.

📈 Key Benefits
Speed

Clarity

Automatable structure

Designed specifically for AI collaboration

Accessible to non-programmers

## 🚧 Next Steps

### Version 0.2 – Planned Enhancements
- Syntax validation and structural consistency checks
- Expansion of language constructs (e.g. conditionals, loops, modular blocks)

### Tooling
- Parser implementation (as open-source CLI or internal utility)
- Web-based editor with live preview and AI-assisted suggestions

### Pilot Testing in Real Use Cases
- Initial deployment and feedback collection in selected domains:
  - Marketing (prompt scripting, automation)
  - Human Resources (feedback forms, onboarding flows)
  - Healthcare (structured protocols, AI-enhanced instructions)


Copyright © 2025 Michal Beran

