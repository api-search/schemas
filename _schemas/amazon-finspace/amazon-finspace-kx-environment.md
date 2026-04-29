---
description: Represents an Amazon FinSpace managed kdb (kdb+/q) environment.
layout: schema
name: KxEnvironment
properties_list:
- description: ''
  name: environmentId
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: awsAccountId
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: tgwStatus
  type: string
- description: ''
  name: dnsStatus
  type: string
- description: ''
  name: errorMessage
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: environmentArn
  type: string
- description: ''
  name: kmsKeyId
  type: string
- description: ''
  name: dedicatedServiceAccountId
  type: string
- description: ''
  name: transitGatewayConfiguration
  type: object
- description: ''
  name: customDNSConfiguration
  type: array
- description: ''
  name: creationTimestamp
  type: string
- description: ''
  name: updateTimestamp
  type: string
- description: ''
  name: availabilityZoneIds
  type: array
- description: ''
  name: certificateAuthorityArn
  type: string
- description: ''
  name: tags
  type: object
provider_name: Amazon FinSpace
provider_slug: amazon-finspace
schema_file: json-schema/amazon-finspace-kx-environment-schema.json
slug: amazon-finspace-kx-environment
source_filename: amazon-finspace-kx-environment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-finspace/refs/heads/main/json-schema/amazon-finspace-kx-environment-schema.json\",\n  \"title\": \"KxEnvironment\",\n  \"description\": \"Represents an Amazon FinSpace managed kdb (kdb+/q) environment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environmentId\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"awsAccountId\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATE_REQUESTED\",\n        \"CREATING\",\n        \"CREATED\",\n        \"DELETE_REQUESTED\",\n        \"DELETING\",\n        \"DELETED\",\n        \"FAILED_CREATION\",\n        \"FAILED_DELETION\",\n        \"RETRY_DELETION\",\n        \"SUSPENDED\"\n      ]\n    },\n    \"tgwStatus\": {\n      \"type\": \"string\"\n    },\n    \"dnsStatus\"\
  : {\n      \"type\": \"string\"\n    },\n    \"errorMessage\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"environmentArn\": {\n      \"type\": \"string\"\n    },\n    \"kmsKeyId\": {\n      \"type\": \"string\"\n    },\n    \"dedicatedServiceAccountId\": {\n      \"type\": \"string\"\n    },\n    \"transitGatewayConfiguration\": {\n      \"type\": \"object\"\n    },\n    \"customDNSConfiguration\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"creationTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updateTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"availabilityZoneIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"certificateAuthorityArn\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"object\"\
  ,\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"kmsKeyId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-finspace/refs/heads/main/json-schema/amazon-finspace-kx-environment-schema.json
tags:
- AWS
- Capital Markets
- Data Analytics
- Data Management
- Financial Services
title: KxEnvironment
---
