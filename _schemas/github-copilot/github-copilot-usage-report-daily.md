---
description: Download links for a daily Copilot usage metrics report.
layout: schema
name: UsageReportDaily
properties_list:
- description: Signed URLs to download the report files.
  name: download_links
  type: array
- description: The date the report covers.
  name: report_day
  type: string
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-usage-report-daily-schema.json
slug: github-copilot-usage-report-daily
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UsageReportDaily\",\n  \"type\": \"object\",\n  \"description\": \"Download links for a daily Copilot usage metrics report.\",\n  \"properties\": {\n    \"download_links\": {\n      \"type\": \"array\",\n      \"description\": \"Signed URLs to download the report files.\"\n    },\n    \"report_day\": {\n      \"type\": \"string\",\n      \"description\": \"The date the report covers.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-usage-report-daily-schema.json
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
title: UsageReportDaily
---
