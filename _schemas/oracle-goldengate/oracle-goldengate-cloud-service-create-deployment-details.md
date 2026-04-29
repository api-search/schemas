---
description: ''
layout: schema
name: CreateDeploymentDetails
properties_list:
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
  name: oggData
  type: object
- description: ''
  name: freeformTags
  type: object
- description: ''
  name: definedTags
  type: object
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-cloud-service-create-deployment-details-schema.json
slug: oracle-goldengate-cloud-service-create-deployment-details
source_filename: oracle-goldengate-cloud-service-create-deployment-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateDeploymentDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\"\n    },\n    \"subnetId\": {\n      \"type\": \"string\"\n    },\n    \"licenseModel\": {\n      \"type\": \"string\"\n    },\n    \"fqdn\": {\n      \"type\": \"string\"\n    },\n    \"cpuCoreCount\": {\n      \"type\": \"integer\"\n    },\n    \"isAutoScalingEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"isPublic\": {\n      \"type\": \"boolean\"\n    },\n    \"oggData\": {\n      \"type\": \"object\"\n    },\n    \"freeformTags\": {\n      \"type\": \"object\"\n    },\n    \"definedTags\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-cloud-service-create-deployment-details-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: CreateDeploymentDetails
---
