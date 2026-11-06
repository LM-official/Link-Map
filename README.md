<div align="center">

# 🗺️ Link-map
**A personal knowledge base** — a _digital garden_ of ideas and resources gathered through online research and published as an interactive graph.

![Entries](https://img.shields.io/badge/Entries-102-4c1?style=flat-square)
![Hubs](https://img.shields.io/badge/Hubs-6-284b63?style=flat-square)
![Language](https://img.shields.io/badge/Notes-Italian-008C45?style=flat-square)
![Language](https://img.shields.io/badge/Notes-English-008C45?style=flat-square)
![License](https://img.shields.io/badge/Content-mixed%20copyright-lightgrey?style=flat-square)

**[→ Explore the live graph](https://lm-official.github.io/Link-Map)**

> [!WARNING] These notes collect publicly available information for personal study. **I am not the owner of the content displayed.**

</div>

---

## 📖 Overview
Link-map collects explanations, questions, guides, and useful tools. Notes are curated in Visual Studio Code and published with [Quartz v4](https://quartz.jzhao.xyz).

Each entry has one primary place in the garden. Annotated connections link related subjects across that structure. A resource collection can hold several bookmarks under useful headings; a new external link does not need its own graph node.

---

## 🌍 Start with a subject
[Home](content/index.md) leads to five broad domains:

| Domain                                                                       | What belongs here                                                      |
| :--------------------------------------------------------------------------- | :--------------------------------------------------------------------- |
| [💻 Computing & Technology](content/HUBS/COMPUTING_TECHNOLOGY.md)            | Programming, systems, databases, security, AI, and robotics            |
| [🧮 Mathematics & Logic](content/HUBS/MATHEMATICS_LOGIC.md)                  | Numbers, computation, geometry, probability, logic, and puzzles        |
| [🔬 Science, Nature & Health](content/HUBS/SCIENCE_NATURE_HEALTH.md)         | Living systems, health, materials, the environment, physics, and space |
| [🏛️ Society, History & Economy](content/HUBS/SOCIETY_HISTORY_ECONOMY.md)     | Society, history, business, personal finance, and internet culture     |
| [🎨 Arts, Design & Communication](content/HUBS/ARTS_DESIGN_COMMUNICATION.md) | Visual and product design, film, photography, sound, and language      |

[Web Development](content/HUBS/WEB_DEVELOPMENT.md) is a topic hub within Computing & Technology. Other topics appear as sections within their domain pages.

[Study resources](content/data/studyResources.md) is a collection linked directly from Home for academic search, LaTeX, university material, archives, and document utilities.

---

## 🕸️ Navigation and the graph
The usual navigation path is **Home → domain → entry**, with optionals topic hubs between a domain and its entries. Hub headings and annotated links give a stable reading order. The force-directed graph is for exploring connections; its positions can change as the garden grows.

| Layer                        | Color | Tag                              | Role                                                           |
| :--------------------------- | :---: | :------------------------------- | :------------------------------------------------------------- |
| Home                         |  🔴   | `hubLvl0`                        | Entry point for the whole garden                               |
| Domain                       |  🟢   | `hubLvl1`                        | One of the five broad subject areas                            |
| Topic hub                    |  🔵   | `hubLvl2`                        | An overview of a substantial topic
| Entry or resource collection |  ⚪   | `documentary` · `guide` · `tool` | An independently useful subject or a set of related references |

Type tags describe what an entry contains, not its subject. They are available for browsing and hidden as nodes in both local and global graphs.

An entry's primary home is the hub or collection that lists it as part of its subject outline. Other links belong in an annotated `Connections` section and explain why the relationship helps. For example, wet collodion lives under Photography and connects to chemistry; AI costs live under Economics and connect to neural networks.

---

## 🌱 Adding entries
1. **Another source for an existing subject?** Add it to that entry.
2. **A brief reference for an existing collection?** Add an annotated item or section.
3. **A distinct question or subject worth revisiting independently?** Create an entry and list it under its primary home.
4. **A collection difficult to scan?** Split out the parts that have developed their own identity.

Group references you would usually consult together. Give a subject its own entry when you would search for, explain, or link to it independently. CGI, stop motion, and motion capture each have an entry with connections to related techniques.

Choose a primary home by where you would expect to find the entry again. Keep a topic as a heading before creating a new hub, and explain each hub's scope in its opening paragraph. A `Connections` link should say what the relationship is; being broadly related is not enough.

---

## 🏷️ Files and titles
- `content/index.md` is Home.
- `content/HUBS/` holds the six hub pages, using `UPPER_SNAKE_CASE` filenames.
- `content/data/` contains entries and resource collections in a flat folder, using `camelCase` filenames.
- Every page has a readable `title` in YAML frontmatter. Quartz renders this as the page title.
- Entries use one or more of `documentary`, `guide`, and `tool`. Hubs use their navigation-level tag.
- Wiki links point to canonical filenames. Display labels and section anchors make the links readable and specific.

---

## 🛠️ Build locally
Use Node.js 22 or newer and npm 10.9.2 or newer:

```sh
npm ci
npx quartz build --serve
```

Before publishing, build Quartz and check that internal links and section anchors resolve and all entries can be reached from Home. Keep the entry and hub badges above in sync with the Markdown files under `content/data/` and `content/HUBS/`.

---
## 👥 Authors
LinkMap was designed and built by:
- **[LM-official](https://github.com/LM-official)**
- **[jackyzha0](https://github.com/jackyzha0/quartz)**

---

## 📄 License
Released under the MIT License. See [LICENSE](LICENSE).