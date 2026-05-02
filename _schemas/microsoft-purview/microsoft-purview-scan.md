---
description: Represents a scan configuration in the Microsoft Purview scanning service. Scans define how data sources are analyzed to discover and classify data assets.
layout: schema
name: Microsoft Purview Scan
properties_list:
- description: The resource identifier of the scan
  name: id
  type: string
- description: The name of the scan
  name: name
  type: string
- description: The type of scan matching the data source kind
  name: kind
  type: string
- description: Scan configuration properties
  name: properties
  type: object
provider_name: Microsoft Purview
provider_slug: microsoft-purview
schema_file: json-schema/microsoft-purview-scan-schema.json
slug: microsoft-purview-scan
source_filename: microsoft-purview-scan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/microsoft-purview/json-schema/microsoft-purview-scan-schema.json\",\n  \"title\": \"Microsoft Purview Scan\",\n  \"description\": \"Represents a scan configuration in the Microsoft Purview scanning service. Scans define how data sources are analyzed to discover and classify data assets.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The resource identifier of the scan\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the scan\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The type of scan matching the data source kind\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Scan configuration properties\",\n      \"properties\": {\n        \"scanRulesetName\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The name of the scan ruleset to use\"\n        },\n        \"scanRulesetType\": {\n          \"type\": \"string\",\n          \"description\": \"Whether the ruleset is custom or system-defined\",\n          \"enum\": [\"Custom\", \"System\"]\n        },\n        \"collection\": {\n          \"type\": \"object\",\n          \"description\": \"The collection to store discovered assets in\",\n          \"properties\": {\n            \"referenceName\": {\n              \"type\": \"string\"\n            },\n            \"type\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"connectedVia\": {\n          \"type\": \"object\",\n          \"description\": \"The integration runtime connection information\",\n          \"properties\": {\n            \"referenceName\": {\n              \"type\": \"string\"\n            },\n            \"integrationRuntimeType\": {\n              \"type\":\
  \ \"string\"\n            }\n          }\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"lastModifiedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"lastScheduled\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    }\n  },\n  \"required\": [\"name\", \"kind\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/json-schema/microsoft-purview-scan-schema.json
tags:
- Compliance
- Data Catalog
- Data Classification
- Data Governance
- Data Loss Prevention
- Information Protection
title: Microsoft Purview Scan
---
