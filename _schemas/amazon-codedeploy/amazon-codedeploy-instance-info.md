---
description: Information about an on-premises instance.
layout: schema
name: InstanceInfo
properties_list:
- description: ''
  name: instanceName
  type: object
- description: ''
  name: iamSessionArn
  type: object
- description: ''
  name: iamUserArn
  type: object
- description: ''
  name: instanceArn
  type: object
- description: ''
  name: registerTime
  type: object
- description: ''
  name: deregisterTime
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-instance-info-schema.json
slug: amazon-codedeploy-instance-info
source_filename: amazon-codedeploy-instance-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-instance-info-schema.json\",\n  \"title\": \"InstanceInfo\",\n  \"description\": \"Information about an on-premises instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceName\"\n        },\n        {\n          \"description\": \"The name of the on-premises instance.\"\n        }\n      ]\n    },\n    \"iamSessionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamSessionArn\"\n        },\n        {\n          \"description\": \"The ARN of the IAM session associated with the on-premises instance.\"\n        }\n      ]\n    },\n    \"iamUserArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamUserArn\"\n\
  \        },\n        {\n          \"description\": \"The IAM user ARN associated with the on-premises instance.\"\n        }\n      ]\n    },\n    \"instanceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceArn\"\n        },\n        {\n          \"description\": \"The ARN of the on-premises instance.\"\n        }\n      ]\n    },\n    \"registerTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the on-premises instance was registered.\"\n        }\n      ]\n    },\n    \"deregisterTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"If the on-premises instance was deregistered, the time at which the on-premises instance was deregistered.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The tags currently associated with the on-premises instance.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-instance-info-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: InstanceInfo
---
