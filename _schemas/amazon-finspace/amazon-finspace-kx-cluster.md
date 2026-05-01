---
description: Represents a cluster of compute resources in a FinSpace kdb environment.
layout: schema
name: KxCluster
properties_list:
- description: ''
  name: clusterName
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: statusReason
  type: string
- description: ''
  name: clusterType
  type: string
- description: ''
  name: tickerplantLogConfiguration
  type: object
- description: ''
  name: volumes
  type: array
- description: ''
  name: databases
  type: array
- description: ''
  name: cacheStorageConfigurations
  type: array
- description: ''
  name: autoScalingConfiguration
  type: object
- description: ''
  name: clusterDescription
  type: string
- description: ''
  name: capacityConfiguration
  type: object
- description: ''
  name: releaseLabel
  type: string
- description: ''
  name: vpcConfiguration
  type: object
- description: ''
  name: initializationScript
  type: string
- description: ''
  name: commandLineArguments
  type: array
- description: ''
  name: code
  type: object
- description: ''
  name: executionRole
  type: string
- description: ''
  name: lastModifiedTimestamp
  type: string
- description: ''
  name: savedownStorageConfiguration
  type: object
- description: ''
  name: azMode
  type: string
- description: ''
  name: availabilityZoneId
  type: string
- description: ''
  name: createdTimestamp
  type: string
- description: ''
  name: tags
  type: object
provider_name: Amazon FinSpace
provider_slug: amazon-finspace
schema_file: json-schema/amazon-finspace-kx-cluster-schema.json
slug: amazon-finspace-kx-cluster
source_filename: amazon-finspace-kx-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-finspace/refs/heads/main/json-schema/amazon-finspace-kx-cluster-schema.json\",\n  \"title\": \"KxCluster\",\n  \"description\": \"Represents a cluster of compute resources in a FinSpace kdb environment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clusterName\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PENDING\",\n        \"CREATING\",\n        \"CREATE_FAILED\",\n        \"RUNNING\",\n        \"UPDATING\",\n        \"DELETING\",\n        \"DELETED\",\n        \"DELETE_FAILED\"\n      ]\n    },\n    \"statusReason\": {\n      \"type\": \"string\"\n    },\n    \"clusterType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"HDB\",\n        \"RDB\",\n        \"GATEWAY\",\n        \"GP\",\n        \"TICKERPLANT\"\n      ]\n    },\n    \"tickerplantLogConfiguration\"\
  : {\n      \"type\": \"object\"\n    },\n    \"volumes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"databases\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"cacheStorageConfigurations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"autoScalingConfiguration\": {\n      \"type\": \"object\"\n    },\n    \"clusterDescription\": {\n      \"type\": \"string\"\n    },\n    \"capacityConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"nodeType\": {\n          \"type\": \"string\"\n        },\n        \"nodeCount\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"releaseLabel\": {\n      \"type\": \"string\"\n    },\n    \"vpcConfiguration\": {\n      \"type\": \"object\"\n    },\n    \"initializationScript\": {\n      \"type\": \"string\"\n    },\n    \"commandLineArguments\"\
  : {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"code\": {\n      \"type\": \"object\"\n    },\n    \"executionRole\": {\n      \"type\": \"string\"\n    },\n    \"lastModifiedTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"savedownStorageConfiguration\": {\n      \"type\": \"object\"\n    },\n    \"azMode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SINGLE\",\n        \"MULTI\"\n      ]\n    },\n    \"availabilityZoneId\": {\n      \"type\": \"string\"\n    },\n    \"createdTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"clusterName\",\n    \"clusterType\",\n    \"capacityConfiguration\",\n    \"releaseLabel\",\n    \"azMode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-finspace/refs/heads/main/json-schema/amazon-finspace-kx-cluster-schema.json
tags:
- Capital Markets
- Data Analytics
- Data Management
- Financial Services
title: KxCluster
---
