---
description: StackDriftInformation schema
layout: schema
name: StackDriftInformation
properties_list:
- description: ''
  name: StackDriftStatus
  type: string
- description: ''
  name: LastCheckTimestamp
  type: string
provider_name: Amazon CloudFormation
provider_slug: amazon-cloudformation
schema_file: json-schema/cloudformation-stack-drift-information-schema.json
slug: cloudformation-stack-drift-information
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-stack-drift-information-schema.json\",\n  \"title\": \"StackDriftInformation\",\n  \"description\": \"StackDriftInformation schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StackDriftStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"DRIFTED\",\n        \"IN_SYNC\",\n        \"UNKNOWN\",\n        \"NOT_CHECKED\"\n      ]\n    },\n    \"LastCheckTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\n    \"StackDriftStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-stack-drift-information-schema.json
tags:
- AWS
- CloudFormation
- Infrastructure as Code
- DevOps
- IaC
title: StackDriftInformation
---
