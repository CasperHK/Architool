# Architool
AI-ready project scaffolding CLI using [Cobra](https://cobra.dev/) for fast setup, automatic documentation, and agent-friendly standards.


Architool helps teams bootstrap consistent project structures with:

* production-minded folder layouts
* auto-generated docs
* built-in conventions for humans and AI agents
* validation and deployment helpers

## Why Architool
Modern teams need more than file generation.
They need structure, documentation, and machine-readable guidance from day one.

Architool creates:

* code structure
* docs structure
* agent instruction scaffolding
* validation workflows
* Docker support
* optional static docs publishing setup

## Core Features
* Project bootstrap in one command
* Bilingual docs structure (English and Traditional Chinese)
* mdBook-ready documentation skeleton
* Agent instruction and skill file generation
* Convention checks for structure and docs parity
* Local docs server and static export support
* Optional GitHub Pages deployment pipeline

## Quick Start
Install:
```
pip install forgepilot
```

Create a project:
```
architool init my-app --docs --langs en,zh-hk
```

Start docs locally:
```
architool docs serve
```

Build docs:
```
architool docs build
```

Validate project conventions:
```
architool validate
```

Command Overview
```
architool init
```

Create new project scaffold with selected modules and docs options
```
architool add
```

Add a feature/module into an existing project with matching docs pages
```
architool docs serve
```

Start docs web server for local preview
```
architool docs build
```

Export static documentation site
```
architool docs sync
```

Check docs structure and language parity
```
architool validate
```

Run structural and policy checks

## Default Project Structure
```
src/
tests/
docs/
book.toml
src/
SUMMARY.md
en/
zh-hk/
.github/
workflows/
instructions/
skills/
pyproject.toml
README.md
```

## Documentation Model
ForgePilot uses mdBook-friendly layout by default:

* docs/src/en for English
* docs/src/zh-hk for Traditional Chinese
* SUMMARY.md as navigation source of truth

When adding a chapter in English, create the corresponding zh-hk chapter in the same change.

## AI-Ready Governance
ForgePilot can generate:

* instruction files for coding agents
* reusable skill files for domain workflows
* project conventions for docs and structure quality gates
* This helps agents and developers follow the same standards consistently.

# Configuration
You can define defaults in a project config file such as:

* preferred languages
* module templates
* doc policies
* CI/deployment preferences
* naming rules

## Roadmap
* Template marketplace
* Plugin system for custom generators
* Built-in migration assistant
* Team policy packs
* Multi-runtime support (Python and Go)

## Contributing
Contributions are welcome.
Recommended flow:

1. Open an issue with proposal
2. Submit focused PR with tests and docs update
3. Keep generated structure and docs parity intact

## License
MIT License
