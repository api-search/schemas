---
description: StackResourceDriftInformation schema
layout: schema
name: StackResourceDriftInformation
properties_list:
- description: ''
  name: StackResourceDriftStatus
  type: string
- description: ''
  name: LastCheckTimestamp
  type: string
provider_name: Amazon CloudFormation
provider_slug: amazon-cloudformation
schema_file: json-schema/cloudformation-stack-resource-drift-information-schema.json
slug: cloudformation-stack-resource-drift-information
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-stack-resource-drift-information-schema.json\",\n  \"title\": \"StackResourceDriftInformation\",\n  \"description\": \"StackResourceDriftInformation schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StackResourceDriftStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"IN_SYNC\",\n        \"MODIFIED\",\n        \"DELETED\",\n        \"NOT_CHECKED\"\n      ]\n    },\n    \"LastCheckTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\n    \"StackResourceDriftStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-stack-resource-drift-information-schema.json
tags:
- AWS
- CloudFormation
- Infrastructure as Code
- DevOps
- IaC
title: StackResourceDriftInformation
---
