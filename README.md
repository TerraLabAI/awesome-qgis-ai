# Awesome QGIS AI [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A plain list of plugins, servers, benchmarks and papers for using AI with QGIS. Maintained by [TerraLab](https://terra-lab.ai), which makes three of the plugins below (marked **maker**). Every other entry is listed on the same terms: what it is, how it gets a model, where it lives. Pull requests from any author are welcome, see [CONTRIBUTING.md](CONTRIBUTING.md).

Counts change fast. On 26 September 2026 the official QGIS plugin list held 38 plugins where a language model acts on QGIS or answers about your project; our method and the full table are in [What is an AI agent in QGIS](https://terra-lab.ai/blog/what-is-an-ai-agent-in-qgis).

## Contents

- [Agents inside QGIS](#agents-inside-qgis)
- [MCP bridges](#mcp-bridges)
- [Segmentation and detection](#segmentation-and-detection)
- [Image editing](#image-editing)
- [Benchmarks and papers](#benchmarks-and-papers)
- [How to choose](#how-to-choose)

## Agents inside QGIS

A chat panel in QGIS that runs the steps in your project.

- [AI Agent by TerraLab](https://plugins.qgis.org/plugins/AI_Agent/) (**maker**): model included, free plan, asks before risky steps, one-click undo. [Source mirror](https://github.com/TerraLabAI/QGIS_AI-Agent).
- [qgis-whitebox-agent](https://github.com/opengeos/qgis-whitebox-agent) by Qiusheng Wu: open source, your own key or a local model.
- [buntinglabs-qgis-plugin](https://github.com/BuntingLabs/buntinglabs-qgis-plugin) by Bunting Labs: vendor account.
- [qgis-ai-agent](https://github.com/mzarov/qgis-ai-agent) by mzarov.
- [QGPTAgent](https://github.com/momaabna/QGPTAgent) by momaabna.

## MCP bridges

QGIS exposes its functions to an outside AI app such as Claude Code, Codex or Cursor through the Model Context Protocol.

- [QGIS MCP](https://plugins.qgis.org/plugins/qgis_mcp_plugin/) by Nicolas Karasiak, with the [server](https://github.com/nkarasiak/qgis-mcp).
- [qgis_mcp](https://github.com/jjsantos01/qgis_mcp) by jjsantos01.
- [TerraLab MCP](https://github.com/TerraLabAI/mcp) (**maker**): hosted, read-only geodata for any place (map data, terrain, routes, satellite images, French parcels) as GIS files that open in QGIS.
- [geoai-skills](https://github.com/TerraLabAI/geoai-skills) (**maker**): agent skills for CRS, PyQGIS for QGIS 4, Sentinel-2 indices, open imagery and map data.

## Segmentation and detection

- [AI Segmentation by TerraLab](https://plugins.qgis.org/plugins/AI_Segmentation/) (**maker**): click one object for its outline, or name what you want for every match in a drawn area. [Source mirror](https://github.com/TerraLabAI/QGIS_AI-Segmentation).
- [Geo-SAM](https://github.com/coolzhao/Geo-SAM) by coolzhao.
- [qgis-samgeo-plugin](https://github.com/opengeos/qgis-samgeo-plugin) by opengeos.
- [geoai](https://github.com/opengeos/geoai) by opengeos: Python package for geospatial AI, used from QGIS and notebooks.

## Image editing

- [AI Edit by TerraLab](https://plugins.qgis.org/plugins/AI_Edit/) (**maker**): edit your aerial imagery from a written instruction, georeferenced output marked as AI-generated. [Source mirror](https://github.com/TerraLabAI/QGIS_AI-Edit).

## Benchmarks and papers

Each benchmark has its own questions and grader, so scores do not compare across them.

- [GeoKTools and GeoExpertQueries](https://github.com/google-research/geospatial-reasoning-benchmarks), Google Research, with the paper [arXiv:2610.15750](https://arxiv.org/abs/2610.15750).
- [GeoBenchX](https://github.com/Solirinai/GeoBenchX), [arXiv:2503.18129](https://arxiv.org/abs/2503.18129): multistep GIS tasks on open data.
- [GeoAnalystBench](https://github.com/GeoDS/GeoAnalystBench): 50 spatial-analysis tasks.
- [GS-QA2](https://huggingface.co/datasets/Zoe/GS-QA2): spatial questions about US places, by Shang et al.
- [GISAgentBench](https://arxiv.org/abs/2608.01645) and [GeoNatureAgent](https://arxiv.org/abs/2610.09112).
- Our own run of four QGIS setups on Google's benchmarks, with method and limits: [AI Agent QGIS plugin benchmark](https://terra-lab.ai/blog/ai-agent-qgis-plugin-geospatial-benchmark). Vendor run, not a leaderboard.

## How to choose

| If you want | Look at |
| --- | --- |
| The result in your open project, nothing to configure | a plugin that includes the model |
| QGIS as one more tool in Claude Code or Cursor | an MCP bridge |
| Nothing leaving your computer | a plugin with a local model, and a strong GPU |
| Your own OpenAI or Anthropic key | a plugin that takes your key |

## Contributing

Add a plugin, server, benchmark or paper with one line: name, author, how it gets a model, link. Say if you are the maker. We check that the link works and the entry is about QGIS and AI; we do not rank.
