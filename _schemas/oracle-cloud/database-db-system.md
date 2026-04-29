---
description: A DB system.
layout: schema
name: DbSystem
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: compartmentId
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: shape
  type: string
- description: ''
  name: availabilityDomain
  type: string
- description: ''
  name: cpuCoreCount
  type: integer
- description: ''
  name: nodeCount
  type: integer
- description: ''
  name: dataStorageSizeInGBs
  type: integer
- description: ''
  name: databaseEdition
  type: string
- description: ''
  name: lifecycleState
  type: string
- description: ''
  name: timeCreated
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/database-db-system-schema.json
slug: database-db-system
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/database-db-system-schema.json\",\n  \"title\": \"DbSystem\",\n  \"description\": \"A DB system.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"my-resource\"\n    },\n    \"shape\": {\n      \"type\": \"string\",\n      \"example\": \"VM.Standard.E4.Flex\"\n    },\n    \"availabilityDomain\": {\n      \"type\": \"string\",\n      \"example\": \"Uocm:US-ASHBURN-AD-1\"\n    },\n    \"cpuCoreCount\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"nodeCount\": {\n      \"type\":\
  \ \"integer\",\n      \"example\": 1\n    },\n    \"dataStorageSizeInGBs\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"databaseEdition\": {\n      \"type\": \"string\",\n      \"enum\": \"['STANDARD_EDITION', 'ENTERPRISE_EDITION', 'ENTERPRISE_EDITION_HIGH_PERFORMANCE', 'ENTERPRISE_EDITION_EXTREME_PERFORMANCE']\",\n      \"example\": \"STANDARD_EDITION\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/database-db-system-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: DbSystem
---
