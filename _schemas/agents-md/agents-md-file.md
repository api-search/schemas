---
description: Representation of an AGENTS.md file's structured content providing context and instructions to AI coding agents.
layout: schema
name: AgentsMdFile
properties_list:
- description: The filename, typically AGENTS.md.
  name: filename
  type: string
- description: File path within the repository.
  name: location
  type: string
- description: Name of the project or subproject this file applies to.
  name: project_name
  type: string
- description: Brief description of the project's purpose and architecture.
  name: description
  type: string
- description: Commands for building the project.
  name: build_commands
  type: array
- description: Commands for running tests.
  name: test_commands
  type: array
- description: Commands for linting and formatting code.
  name: lint_commands
  type: array
- description: Coding conventions and style guidelines for the project.
  name: coding_standards
  type: array
- description: Security considerations and sensitive file locations agents should be aware of.
  name: security_notes
  type: array
- description: Date the AGENTS.md file was created.
  name: created
  type: string
- description: Date the AGENTS.md file was last modified.
  name: modified
  type: string
provider_name: AGENTS.md
provider_slug: agents-md
schema_file: json-schema/agents-md-file-schema.json
slug: agents-md-file
source_filename: agents-md-file-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agents-md/refs/heads/main/json-schema/agents-md-file-schema.json\",\n  \"title\": \"AgentsMdFile\",\n  \"description\": \"Representation of an AGENTS.md file's structured content providing context and instructions to AI coding agents.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filename\": {\n      \"type\": \"string\",\n      \"description\": \"The filename, typically AGENTS.md.\",\n      \"example\": \"AGENTS.md\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"File path within the repository.\",\n      \"example\": \"/AGENTS.md\"\n    },\n    \"project_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the project or subproject this file applies to.\",\n      \"example\": \"My API Service\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Brief description of the project's purpose and architecture.\",\n      \"example\": \"A REST API service built with FastAPI and PostgreSQL.\"\n    },\n    \"build_commands\": {\n      \"type\": \"array\",\n      \"description\": \"Commands for building the project.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"label\": { \"type\": \"string\", \"example\": \"Install dependencies\" },\n          \"command\": { \"type\": \"string\", \"example\": \"pip install -r requirements.txt\" }\n        }\n      }\n    },\n    \"test_commands\": {\n      \"type\": \"array\",\n      \"description\": \"Commands for running tests.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"label\": { \"type\": \"string\", \"example\": \"Run unit tests\" },\n          \"command\": { \"type\": \"string\", \"example\": \"pytest tests/ -v\" }\n        }\n      }\n    },\n    \"lint_commands\": {\n      \"type\": \"array\"\
  ,\n      \"description\": \"Commands for linting and formatting code.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"label\": { \"type\": \"string\", \"example\": \"Lint code\" },\n          \"command\": { \"type\": \"string\", \"example\": \"ruff check . && black --check .\" }\n        }\n      }\n    },\n    \"coding_standards\": {\n      \"type\": \"array\",\n      \"description\": \"Coding conventions and style guidelines for the project.\",\n      \"items\": { \"type\": \"string\" },\n      \"example\": [\"Use snake_case for Python identifiers\", \"Keep functions under 50 lines\"]\n    },\n    \"security_notes\": {\n      \"type\": \"array\",\n      \"description\": \"Security considerations and sensitive file locations agents should be aware of.\",\n      \"items\": { \"type\": \"string\" },\n      \"example\": [\"Never commit .env files\", \"Secrets are stored in AWS Secrets Manager\"]\n    },\n    \"created\": {\n      \"type\": \"\
  string\",\n      \"format\": \"date\",\n      \"description\": \"Date the AGENTS.md file was created.\",\n      \"example\": \"2026-01-15\"\n    },\n    \"modified\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the AGENTS.md file was last modified.\",\n      \"example\": \"2026-04-19\"\n    }\n  },\n  \"required\": [\"filename\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agents-md/refs/heads/main/json-schema/agents-md-file-schema.json
tags:
- AI Agents
- AI Copilot
- Coding Standards
- Developer Workflow
- Open Standard
- Documentation
title: AgentsMdFile
---
