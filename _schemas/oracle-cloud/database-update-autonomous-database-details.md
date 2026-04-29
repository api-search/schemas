---
description: UpdateAutonomousDatabaseDetails schema from oracle-cloud-database-openapi.yaml
layout: schema
name: UpdateAutonomousDatabaseDetails
properties_list:
- description: ''
  name: displayName
  type: string
- description: ''
  name: cpuCoreCount
  type: integer
- description: ''
  name: dataStorageSizeInTBs
  type: integer
- description: ''
  name: isAutoScalingEnabled
  type: boolean
- description: ''
  name: adminPassword
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/database-update-autonomous-database-details-schema.json
slug: database-update-autonomous-database-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/database-update-autonomous-database-details-schema.json\",\n  \"title\": \"UpdateAutonomousDatabaseDetails\",\n  \"description\": \"UpdateAutonomousDatabaseDetails schema from oracle-cloud-database-openapi.yaml\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"my-resource\"\n    },\n    \"cpuCoreCount\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"dataStorageSizeInTBs\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"isAutoScalingEnabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"adminPassword\": {\n      \"type\": \"string\",\n      \"format\": \"password\",\n      \"example\": \"********\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/database-update-autonomous-database-details-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: UpdateAutonomousDatabaseDetails
---
