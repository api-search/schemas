---
description: ''
layout: schema
name: KeyTransactionLinksResponse
properties_list:
- description: Application from which this key transaction originated
  name: application
  type: integer
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-key-transaction-links-response-schema.json
slug: new-relic-key-transaction-links-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"application\": {\n      \"type\": \"integer\",\n      \"description\": \"Application from which this key transaction originated\",\n      \"example\": 100\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeyTransactionLinksResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-key-transaction-links-response-schema.json
tags:
- Analysis
- Analytics
- APM
- DevOps
- Infrastructure
- Monitoring
- Observability
- Performance
- Platform
title: KeyTransactionLinksResponse
---
