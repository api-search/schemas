---
description: ''
layout: schema
name: DistributionPath
properties_list:
- description: Distribution path name
  name: name
  type: string
- description: ''
  name: status
  type: string
- description: Source trail file
  name: source
  type: string
- description: Target receiver URL
  name: target
  type: string
- description: Target data type
  name: targetType
  type: string
- description: Filter rule name
  name: ruleName
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-distribution-path-schema.json
slug: oracle-goldengate-rest-distribution-path
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DistributionPath\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Distribution path name\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Source trail file\"\n    },\n    \"target\": {\n      \"type\": \"string\",\n      \"description\": \"Target receiver URL\"\n    },\n    \"targetType\": {\n      \"type\": \"string\",\n      \"description\": \"Target data type\"\n    },\n    \"ruleName\": {\n      \"type\": \"string\",\n      \"description\": \"Filter rule name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-distribution-path-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: DistributionPath
---
