# Welcome to FastOMOP

## Observational Medical Outcomes Partnership Common Data Model

The [OMOP Common Data Model (CDM)](https://www.ohdsi.org/data-standardization/) is a standardized data model designed to organize healthcare data into a common structure. It enables systematic analysis across disparate observational databases and facilitates collaborative research in the healthcare domain.

## Model Context Protocol

[The Model Context Protocol (MCP)](https://modelcontextprotocol.io/) is a framework that enables structured interaction between Large Language Models (LLMs) and databases. OMCP combines this protocol with the OMOP data model to create a powerful system for healthcare data analysis.

## What is OMCP?

OMCP (OMOP Model Context Protocol) is an open-source server that enables Large Language Models (LLMs) to interact with healthcare databases that follow the OMOP Common Data Model. It provides a structured way for AI systems to:

- Query healthcare data with appropriate security and privacy controls
- Perform cohort discovery and selection
- Generate statistical analyses and insights from clinical data
- Maintain data lineage and provenance tracking
- Access standardized healthcare terminologies and concept mappings

### Use Cases

- Clinical research and cohort discovery
- Population health analytics
- Healthcare quality measurement
- Drug safety surveillance
- Clinical decision support
- Medical knowledge extraction

### Architecture

Our first project, [OMCP](https://github.com/fastomop/omcp), is a Model Context Protocol server that sits between LLMs and OMOP CDM databases, providing a structured, secure interface for AI models to query and analyze healthcare data without direct database access.

```
+-------+     +--------------+     +----------------+
|  LLM  | <-> | OMCP Server  | <-> | OMOP Database  |
+-------+     +--------------+     +----------------+
             /                \
   Natural Language      Structured Queries
     Requests            & Data Validation
```
