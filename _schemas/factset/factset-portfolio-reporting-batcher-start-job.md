---
description: Details required to start a job
layout: schema
name: startJob
properties_list:
- description: The name of the PRB job
  name: jobName
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-portfolio-reporting-batcher-start-job-schema.json
slug: factset-portfolio-reporting-batcher-start-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"startJob\",\n  \"type\": \"object\",\n  \"description\": \"Details required to start a job\",\n  \"properties\": {\n    \"jobName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the PRB job\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-portfolio-reporting-batcher-start-job-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: startJob
---
