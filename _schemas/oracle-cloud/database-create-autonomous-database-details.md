---
description: Details for creating an Autonomous Database.
layout: schema
name: CreateAutonomousDatabaseDetails
properties_list:
- description: ''
  name: compartmentId
  type: string
- description: ''
  name: dbName
  type: string
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
  name: adminPassword
  type: string
- description: ''
  name: dbWorkload
  type: string
- description: ''
  name: isFreeTier
  type: boolean
- description: ''
  name: isAutoScalingEnabled
  type: boolean
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/database-create-autonomous-database-details-schema.json
slug: database-create-autonomous-database-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/database-create-autonomous-database-details-schema.json\",\n  \"title\": \"CreateAutonomousDatabaseDetails\",\n  \"description\": \"Details for creating an Autonomous Database.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"compartmentId\",\n    \"dbName\",\n    \"cpuCoreCount\",\n    \"dataStorageSizeInTBs\",\n    \"adminPassword\"\n  ],\n  \"properties\": {\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"dbName\": {\n      \"type\": \"string\",\n      \"example\": \"MYADB\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"my-adb\"\n    },\n    \"cpuCoreCount\": {\n      \"type\": \"integer\",\n      \"example\": 2\n    },\n    \"dataStorageSizeInTBs\": {\n      \"type\": \"integer\"\
  ,\n      \"example\": 1\n    },\n    \"adminPassword\": {\n      \"type\": \"string\",\n      \"format\": \"password\",\n      \"example\": \"********\"\n    },\n    \"dbWorkload\": {\n      \"type\": \"string\",\n      \"enum\": \"['OLTP', 'DW', 'AJD', 'APEX']\",\n      \"example\": \"OLTP\"\n    },\n    \"isFreeTier\": {\n      \"type\": \"boolean\",\n      \"example\": false,\n      \"default\": false\n    },\n    \"isAutoScalingEnabled\": {\n      \"type\": \"boolean\",\n      \"example\": false,\n      \"default\": false\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/database-create-autonomous-database-details-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: CreateAutonomousDatabaseDetails
---
