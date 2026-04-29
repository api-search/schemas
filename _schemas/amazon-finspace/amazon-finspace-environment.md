---
description: Represents an Amazon FinSpace environment for financial analytics workloads.
layout: schema
name: Environment
properties_list:
- description: Unique identifier for the environment.
  name: environmentId
  type: string
- description: Name of the FinSpace environment.
  name: name
  type: string
- description: AWS account ID of the environment owner.
  name: awsAccountId
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: environmentUrl
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: environmentArn
  type: string
- description: ''
  name: sageMakerStudioDomainUrl
  type: string
- description: ''
  name: kmsKeyId
  type: string
- description: ''
  name: dedicatedServiceAccountId
  type: string
- description: ''
  name: federationMode
  type: string
- description: ''
  name: tags
  type: object
provider_name: Amazon FinSpace
provider_slug: amazon-finspace
schema_file: json-schema/amazon-finspace-environment-schema.json
slug: amazon-finspace-environment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-finspace/refs/heads/main/json-schema/amazon-finspace-environment-schema.json\",\n  \"title\": \"Environment\",\n  \"description\": \"Represents an Amazon FinSpace environment for financial analytics workloads.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environmentId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the environment.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the FinSpace environment.\"\n    },\n    \"awsAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"AWS account ID of the environment owner.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATE_REQUESTED\",\n        \"CREATING\",\n        \"CREATED\",\n        \"DELETE_REQUESTED\",\n        \"DELETING\",\n        \"DELETED\"\
  ,\n        \"FAILED_CREATION\",\n        \"FAILED_DELETION\",\n        \"RETRY_DELETION\",\n        \"SUSPENDED\"\n      ]\n    },\n    \"environmentUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"environmentArn\": {\n      \"type\": \"string\"\n    },\n    \"sageMakerStudioDomainUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    },\n    \"kmsKeyId\": {\n      \"type\": \"string\"\n    },\n    \"dedicatedServiceAccountId\": {\n      \"type\": \"string\"\n    },\n    \"federationMode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"FEDERATED\",\n        \"LOCAL\"\n      ]\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-finspace/refs/heads/main/json-schema/amazon-finspace-environment-schema.json
tags:
- AWS
- Capital Markets
- Data Analytics
- Data Management
- Financial Services
title: Environment
---
