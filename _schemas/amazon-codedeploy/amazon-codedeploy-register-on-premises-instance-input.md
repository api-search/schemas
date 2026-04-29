---
description: Represents the input of the register on-premises instance operation.
layout: schema
name: RegisterOnPremisesInstanceInput
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
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-register-on-premises-instance-input-schema.json
slug: amazon-codedeploy-register-on-premises-instance-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-register-on-premises-instance-input-schema.json\",\n  \"title\": \"RegisterOnPremisesInstanceInput\",\n  \"description\": \"Represents the input of the register on-premises instance operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceName\"\n        },\n        {\n          \"description\": \"The name of the on-premises instance to register.\"\n        }\n      ]\n    },\n    \"iamSessionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamSessionArn\"\n        },\n        {\n          \"description\": \"The ARN of the IAM session to associate with the on-premises instance.\"\n        }\n      ]\n    },\n    \"iamUserArn\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamUserArn\"\n        },\n        {\n          \"description\": \"The ARN of the IAM user to associate with the on-premises instance.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"instanceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-register-on-premises-instance-input-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: RegisterOnPremisesInstanceInput
---
