---
description: ''
layout: schema
name: Deployment
properties_list:
- description: OCID of the deployment
  name: id
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: compartmentId
  type: string
- description: ''
  name: subnetId
  type: string
- description: ''
  name: licenseModel
  type: string
- description: ''
  name: fqdn
  type: string
- description: ''
  name: cpuCoreCount
  type: integer
- description: ''
  name: isAutoScalingEnabled
  type: boolean
- description: ''
  name: isPublic
  type: boolean
- description: ''
  name: publicIpAddress
  type: string
- description: ''
  name: privateIpAddress
  type: string
- description: ''
  name: deploymentUrl
  type: string
- description: ''
  name: lifecycleState
  type: string
- description: ''
  name: oggData
  type: object
- description: ''
  name: timeCreated
  type: string
- description: ''
  name: timeUpdated
  type: string
- description: ''
  name: freeformTags
  type: object
- description: ''
  name: definedTags
  type: object
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-cloud-service-deployment-schema.json
slug: oracle-goldengate-cloud-service-deployment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Deployment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"OCID of the deployment\"\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\"\n    },\n    \"subnetId\": {\n      \"type\": \"string\"\n    },\n    \"licenseModel\": {\n      \"type\": \"string\"\n    },\n    \"fqdn\": {\n      \"type\": \"string\"\n    },\n    \"cpuCoreCount\": {\n      \"type\": \"integer\"\n    },\n    \"isAutoScalingEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"isPublic\": {\n      \"type\": \"boolean\"\n    },\n    \"publicIpAddress\": {\n      \"type\": \"string\"\n    },\n    \"privateIpAddress\": {\n      \"type\": \"string\"\n    },\n    \"deploymentUrl\": {\n      \"type\": \"string\"\n    },\n    \"\
  lifecycleState\": {\n      \"type\": \"string\"\n    },\n    \"oggData\": {\n      \"type\": \"object\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\"\n    },\n    \"timeUpdated\": {\n      \"type\": \"string\"\n    },\n    \"freeformTags\": {\n      \"type\": \"object\"\n    },\n    \"definedTags\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-cloud-service-deployment-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: Deployment
---
