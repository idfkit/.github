<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/idfkit/idfkit-brand/releases/download/identity-2026.1/lockup-on-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://github.com/idfkit/idfkit-brand/releases/download/identity-2026.1/lockup-on-light.svg">
    <img alt="idfkit" width="240" src="https://github.com/idfkit/idfkit-brand/releases/download/identity-2026.1/tile.svg">
  </picture>
</p>

Open-source tooling for EnergyPlus building energy simulation, in Python, TypeScript and the browser.

[idfkit](https://idfkit.com) · [Developers](https://developers.idfkit.com) · [EnergyPlus docs](https://docs.idfkit.com) · [Envelop](https://app.idfkit.com) · [MCP](https://mcp.idfkit.com) · [Shoebox](https://shoebox.idfkit.com) · [GitHub](https://github.com/idfkit)

# idfkit

## Repositories

- [idfkit](https://github.com/idfkit/idfkit): An EnergyPlus IDF and epJSON toolkit for Python, with no third-party dependencies.
- [idfkit-js](https://github.com/idfkit/idfkit-js): EnergyPlus IDF and epJSON parsing and manipulation for JavaScript and TypeScript.
- [idfkit-mcp](https://github.com/idfkit/idfkit-mcp): An MCP server that lets an AI assistant author, validate and simulate EnergyPlus models with idfkit.
- [idfkit-lsp](https://github.com/idfkit/idfkit-lsp): A language server and VS Code extension for EnergyPlus development with idfkit.
- [idfkit-plugin](https://github.com/idfkit/idfkit-plugin): A Claude Code and Codex plugin that bundles the idfkit MCP and language servers with skills for EnergyPlus modelling.
- [idfkit-docs](https://github.com/idfkit/idfkit-docs): The EnergyPlus input and output reference, rendered by idfkit for every supported version.
- [idfkit-developers](https://github.com/idfkit/idfkit-developers): The unified idfkit documentation site, for Python and JavaScript alike.
- [idfkit.com](https://github.com/idfkit/idfkit.com): The idfkit website: the front door to the toolkit, the editor, the server and the documentation.
- [idfkit-shoebox](https://github.com/idfkit/idfkit-shoebox): EnergyPlus in the browser: a client-side shoebox model on a drafting sheet.
- [idfkit-conformance](https://github.com/idfkit/idfkit-conformance): The conformance corpus and governance registers that hold idfkit and idfkit-js to one behaviour.
- [idfkit-auth](https://github.com/idfkit/idfkit-auth): The sign-in page for the hosted idfkit services, built on the provider's hosted widget.

## Hosts

- [idfkit.com](https://idfkit.com): the website.
- [developers.idfkit.com](https://developers.idfkit.com): the developer documentation, for Python and JavaScript.
- [docs.idfkit.com](https://docs.idfkit.com): the EnergyPlus input and output reference.
- [app.idfkit.com](https://app.idfkit.com): idfkit Envelop, the web-based EnergyPlus editor.
- [mcp.idfkit.com](https://mcp.idfkit.com): the hosted MCP server.
- [shoebox.idfkit.com](https://shoebox.idfkit.com): Shoebox, EnergyPlus in the browser.
- [auth.idfkit.com](https://auth.idfkit.com): sign-in for the hosted services.

## Quick start

Python:

```bash
pip install idfkit
```

```python
from idfkit import load_idf, save_idf

doc = load_idf("model.idf")
zone = doc["Zone"]["Office"]
zone.name = "Open Plan Office"  # every reference to the zone is updated
save_idf(doc, "updated.idf")
```

JavaScript and TypeScript:

```bash
npm install @idfkit/core @idfkit/schemas
```

The guides and the reference for both languages are at [developers.idfkit.com](https://developers.idfkit.com).
