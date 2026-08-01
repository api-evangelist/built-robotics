# Built Robotics

Built Robotics is a San Francisco robotics company, founded in 2016 by Noah Ready-Campbell and Andrew Liang, that turns conventional heavy construction equipment into AI-powered autonomous robots. Its Exosystem retrofit kit converts excavators and other earthmoving machines into self-operating robots for trenching, foundation excavation and pad grading, while the RPD 35 and RPS 25 autonomous pile drivers install foundations for utility-scale solar farms. Machines are supervised from the Everest command center, and field deployment is run through its Built Solar Technologies (built.solar) division.

- Website: https://www.builtrobotics.com/
- Built Solar Technologies: https://built.solar/
- GitHub: https://github.com/builtrobotics
- Secondary market listing: https://forgeglobal.com/built-robotics_stock/

## API surface

Built Robotics publishes **no public API**. Contract discovery (2026-08-01) probed
`www.builtrobotics.com`, `built.solar` and `everest.builtrobotics.com` for OpenAPI/Swagger,
GraphQL introspection, MCP `tools/list` and A2A agent cards at both well-known paths — all
missed. The company's own `llms.txt` / `llms-full.txt` site inventories contain no developer
or API section, and no public repo in its GitHub organization carries a spec or `.proto`.

What it *does* publish, and what this repo captures:

| Artifact | What was found |
|---|---|
| `llms/` | A real, provider-published `llms.txt` (186 lines), saved verbatim |
| `well-known/` | A real RFC 9116 `security.txt` (expiring), plus `robots.txt` with an explicit AI-agent vs AI-training policy |
| `security/` | Vulnerability-disclosure contact + policy, and a TLS/DNS domain-security probe |
| `packages/` | One first-party open-source package — `rsplan` on PyPI (a Reeds-Shepp path planner). Not an API SDK |
| `conformance/` | Which web/agent discovery standards the company adopts, with evidence |
