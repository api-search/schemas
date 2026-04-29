---
description: An Oracle Autonomous Database.
layout: schema
name: AutonomousDatabase
properties_list:
- description: The OCID.
  name: id
  type: string
- description: The OCID of the compartment.
  name: compartmentId
  type: string
- description: User-friendly name.
  name: displayName
  type: string
- description: The database name.
  name: dbName
  type: string
- description: Number of CPU cores.
  name: cpuCoreCount
  type: integer
- description: Data storage size in terabytes.
  name: dataStorageSizeInTBs
  type: integer
- description: The workload type.
  name: dbWorkload
  type: string
- description: Current state.
  name: lifecycleState
  type: string
- description: Whether this is an Always Free resource.
  name: isFreeTier
  type: boolean
- description: Whether auto scaling is enabled.
  name: isAutoScalingEnabled
  type: boolean
- description: ''
  name: connectionUrls
  type: object
- description: ''
  name: timeCreated
  type: string
- description: ''
  name: freeformTags
  type: object
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/database-autonomous-database-schema.json
slug: database-autonomous-database
source_filename: database-autonomous-database-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/database-autonomous-database-schema.json\",\n  \"title\": \"AutonomousDatabase\",\n  \"description\": \"An Oracle Autonomous Database.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID.\",\n      \"example\": \"ocid1.autonomousdatabase.oc1.iad.abcdefg\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the compartment.\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"User-friendly name.\",\n      \"example\": \"my-adb\"\n    },\n    \"dbName\": {\n      \"type\": \"string\",\n      \"description\": \"The database name.\",\n      \"example\": \"MYADB\"\n    },\n    \"cpuCoreCount\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Number of CPU cores.\",\n      \"example\": 2\n    },\n    \"dataStorageSizeInTBs\": {\n      \"type\": \"integer\",\n      \"description\": \"Data storage size in terabytes.\",\n      \"example\": 1\n    },\n    \"dbWorkload\": {\n      \"type\": \"string\",\n      \"description\": \"The workload type.\",\n      \"enum\": \"['OLTP', 'DW', 'AJD', 'APEX']\",\n      \"example\": \"OLTP\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"description\": \"Current state.\",\n      \"enum\": \"['PROVISIONING', 'AVAILABLE', 'STOPPING', 'STOPPED', 'STARTING', 'TERMINATING', 'TERMINATED', 'RESTORE_IN_PROGRESS', 'BACKUP_IN_PROGRESS', 'SCALE_IN_PROGRESS', 'AVAILABLE_NEEDS_ATTENTION', 'UPDATING']\",\n      \"example\": \"PROVISIONING\"\n    },\n    \"isFreeTier\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is an Always Free resource.\",\n      \"example\": true\n    },\n    \"isAutoScalingEnabled\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether auto scaling is enabled.\",\n      \"example\": true\n    },\n    \"connectionUrls\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"sqlDevWebUrl\": \"example-value\",\n        \"apexUrl\": \"example-value\",\n        \"graphStudioUrl\": \"example-value\"\n      }\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    },\n    \"freeformTags\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key1\": \"value1\"\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/database-autonomous-database-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: AutonomousDatabase
---
