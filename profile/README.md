<h1 align="center">⚡ idfkit</h1>

<p align="center">
  <strong>A modern, open-source toolkit ecosystem for EnergyPlus building energy simulation.</strong>
</p>

<p align="center">
  <a href="https://idfkit.com">Website</a> · <a href="https://docs.idfkit.com">Docs</a> · <a href="https://app.idfkit.com">Web Editor</a> · <a href="https://py.idfkit.com">Python API</a>
</p>

---

idfkit gives you everything you need to model, simulate, and optimize building energy performance — from a fast Python library to a visual web editor to AI-powered automation.

### Ecosystem

| | Repository | Description |
|---|---|---|
| ⚡ | [**idfkit**](https://github.com/idfkit/idfkit) | Core Python toolkit — O(1) lookups, reference tracking, IDF + epJSON, weather, simulation |
| 🏗️ | [**idfkit-app**](https://github.com/idfkit/idfkit-app) | Envelop — browser-native EnergyPlus editor with visual HVAC design and 3D geometry |
| 🤖 | [**idfkit-mcp**](https://github.com/idfkit/idfkit-mcp) | MCP server exposing 25 AI tools for schema, modeling, weather, and simulation |
| 🧠 | [**idfkit-lsp**](https://github.com/idfkit/idfkit-lsp) | Language Server + VS Code extension for intelligent EnergyPlus Python editing |
| 📖 | [**idfkit-docs**](https://github.com/idfkit/idfkit-docs) | Interactive EnergyPlus Input/Output reference documentation |
| 🌐 | [**idfkit.com**](https://github.com/idfkit/idfkit.com) | Project website and ecosystem hub |

### Quick Start

```bash
pip install idfkit
```

```python
from idfkit import load_idf

doc = load_idf("model.idf")
zone = doc["Zone"]["Office"]
zone.name = "Open Plan Office"  # all references update automatically
doc.save("updated.idf")
```

### Highlights

- **4,000x faster** lookups than legacy tools via O(1) indexed collections
- **IDF + epJSON** — read, write, and convert between both formats
- **55,000+ weather stations** — search by location, download EPW/DDY files
- **AI-native** — MCP server with 25 tools for autonomous agent workflows
- **Zero install web editor** — visual HVAC design and in-browser simulation

---

<p align="center">
  <sub>idfkit is in beta — we'd love your <a href="https://github.com/idfkit/idfkit/issues">feedback</a>.</sub>
</p>
