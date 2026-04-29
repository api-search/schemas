---
description: Download links for a 28-day Copilot usage metrics report.
layout: schema
name: UsageReport28Day
properties_list:
- description: Signed URLs to download the report files.
  name: download_links
  type: array
- description: Start date of the 28-day reporting period.
  name: report_start_day
  type: string
- description: End date of the 28-day reporting period.
  name: report_end_day
  type: string
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-usage-report28-day-schema.json
slug: github-copilot-usage-report28-day
source_filename: github-copilot-usage-report28-day-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UsageReport28Day\",\n  \"type\": \"object\",\n  \"description\": \"Download links for a 28-day Copilot usage metrics report.\",\n  \"properties\": {\n    \"download_links\": {\n      \"type\": \"array\",\n      \"description\": \"Signed URLs to download the report files.\"\n    },\n    \"report_start_day\": {\n      \"type\": \"string\",\n      \"description\": \"Start date of the 28-day reporting period.\"\n    },\n    \"report_end_day\": {\n      \"type\": \"string\",\n      \"description\": \"End date of the 28-day reporting period.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-usage-report28-day-schema.json
tags:
- Agents
- AI
- Artificial Intelligence
- Code Generation
- Code Review
- Coding Agent
- Custom Instructions
- Developer Tools
- Extensions
- IDE
- Machine Learning
- MCP
- Metrics
- Model Context Protocol
- Productivity
title: UsageReport28Day
---
