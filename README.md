# 🚀 Power BI Desktop MCP Server

**Version 2.0.9.1**

### *Bring Conversational AI Directly Into Power BI Desktop*

The **Power BI Desktop MCP Server** is the first **AI-native bridge** that lets Claude, GPT, and other MCP-compatible assistants *understand, explore, and even modify* your Power BI models using natural language.

If you've ever wished you could say "Explain this model" or "Show the lineage of power query tables," this is for you.

![Power BI Desktop MCP Server](Asssets/Screenshots/Screenshot%202025-11-30%20053651.png)

## 🎥 Getting Started in 10 Minutes with Agentic BI

Watch our quick tutorial to see the Power BI Desktop MCP Server in action:

<div style="width: 100%;">
  <iframe width="100%" height="500" src="https://www.youtube.com/embed/Xmu1JnsQdB4?start=1" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

---

## 🌟 What It Does

This MCP server turns Power BI Desktop into an AI-accessible platform with:

* **Full model introspection**
  Tables, measures, relationships, Power Query, formats, metadata

* **Write operations**
  Create, update, or remove measures, tables, columns, or relationships

* **Report & visual insights**
  AI-readable report.json, visuals, pages, and layout info

* **Documentation & analysis**
  Auto-generate docs, preview data, run DAX queries, get stats

* **Performance & governance (planned)**
  DAX linting, best-practice scans, compression checks, lineage

It's more than a connector—it's the **AI sidecar for Power BI**.

---

## 🌱 Part of the ABIS Vision

This project is the foundation for **ABIS (Artificial Business Intelligence Services)**—an ecosystem where AI assists with modeling, governance, optimization, and refactoring.

Planned expansions include:

* Multi-model lineage engine
* Enterprise governance & standards
* AI-powered performance tuning
* Team collaboration with AI

Want to shape these features? Reach out—details at the bottom.

---

## 🧩 Capability Snapshot

| Category                                   | Status |
| ------------------------------------------ | ------ |
| Connect & Discover running models          | ✅      |
| Read tables/columns/measures/relationships | ✅      |
| Create/update/delete model objects         | ✅      |
| Inspect reports, pages & visuals           | ✅      |
| Query, stats, documentation                | ✅      |
| Partitions, calc groups, UDFs              | ⏳      |
| Performance, governance, lineage           | ⏳      |

**60+ capabilities** available today.

---

## ⚙️ Installation (Claude Desktop)

1. Place the executable after creating a new folder

   ```
   C:\Program Files\PowerBI-MCP\PbiMcpServerAbisSidecar.exe
   ```

2. Open Claude → Settings → Developer → Edit Config

3. Add:

   ```json
   {
     "mcpServers": {
       "powerbi-desktop": {
         "command": "C:\\Program Files\\PowerBI-MCP\\PbiMcpServerAbisSidecar.exe",
         "args": []
       }
     }
   }
   ```

4. Restart Claude

5. Ask Claude: **"What Power BI models are available?"**

---

## ▶️ Usage

1. Open a PBIX in Power BI Desktop

2. Open Claude Desktop

3. Ask things like:

   * "List all measures"
   * "Explain my report structure"
   * "Generate documentation for this model"
   * "Run a DAX query: EVALUATE Sales"

![Usage Example](Asssets/Screenshots/Screenshot%202025-11-30%20071302.png)

---

## 🩺 Troubleshooting

* No connection → Check path, restart Claude, ensure PBIX is open
* No instances found → Must use the MSI version of Power BI Desktop
* Still stuck? Open an issue or contact us

---

## 💬 Want to Collaborate?

We welcome contributors, ideas, testers, and early adopters.

👉 **Email: [dave@abis-cloud.nl](mailto:dave@abis-cloud.nl)**

👉 **Or open an issue:**

[https://github.com/ABISCloud/powerbi-desktop-mcp-server-abis-sidecar/issues](https://github.com/ABISCloud/powerbi-desktop-mcp-server-abis-sidecar/issues)

👉 **Follow us: [DBI Analytics](https://dbi-analytics.de/)**

Let's build the future of AI-powered BI together.

---

## 📋 Release Notes

### Version 2.0.9.1 (Current)
* Build improvements and stability enhancements

### Version 2.0.9
* **Full Write Operations** - Complete CRUD for tables, columns, measures, and relationships
* **Safety Layer** - Dry-run mode and confirmation flags for destructive operations
* **Enhanced Relationship Support** - Enriched relationship metadata with comprehensive details
* **Report & Visual Inspection** - Full report.json and visual configuration access
* **PBIP & TMDL Support** - Read and parse Power BI Project files and TMDL model definitions
* **Auto Documentation** - Generate comprehensive HTML documentation for entire projects
* **Data Analysis Tools** - Table preview, column statistics, VertiPaq stats, model search
* **Data Source Management** - List and inspect data sources and connection properties

### Version 2.0.8
* **Model Read Operations** - Complete introspection of tables, columns, measures, relationships
* **Metadata Extraction** - Descriptions, format strings, display folders
* **Power Query Support** - Access to M expressions and query definitions
* **DBML Generation** - Export model schema to Database Markup Language format
* **Connection Management** - Discover and connect to Power BI Desktop instances

### Version 2.0.0
* **Initial Release** - Foundation MCP server with basic model connection
* **Core Capabilities** - Port discovery, model connection, basic metadata retrieval
* **MCP Protocol Compliance** - Full compliance with MCP specification

---

## 🔒 Privacy & License

Runs 100% locally. No data leaves your machine.

MIT License — © 2024 ABIS B.V.

Built with ❤️ from engineers for engineers.

---
