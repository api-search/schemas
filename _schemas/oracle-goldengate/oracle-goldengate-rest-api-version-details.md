---
description: ''
layout: schema
name: ApiVersionDetails
properties_list:
- description: ''
  name: version
  type: string
- description: ''
  name: isLatest
  type: boolean
- description: ''
  name: lifecycle
  type: string
- description: ''
  name: links
  type: array
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-api-version-details-schema.json
slug: oracle-goldengate-rest-api-version-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApiVersionDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"string\"\n    },\n    \"isLatest\": {\n      \"type\": \"boolean\"\n    },\n    \"lifecycle\": {\n      \"type\": \"string\"\n    },\n    \"links\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-api-version-details-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: ApiVersionDetails
---
