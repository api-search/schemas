---
description: Represents the input of a <code>DeregisterOnPremisesInstance</code> operation.
layout: schema
name: DeregisterOnPremisesInstanceInput
properties_list:
- description: ''
  name: instanceName
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-deregister-on-premises-instance-input-schema.json
slug: amazon-codedeploy-deregister-on-premises-instance-input
source_filename: amazon-codedeploy-deregister-on-premises-instance-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-deregister-on-premises-instance-input-schema.json\",\n  \"title\": \"DeregisterOnPremisesInstanceInput\",\n  \"description\": \"Represents the input of a <code>DeregisterOnPremisesInstance</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceName\"\n        },\n        {\n          \"description\": \"The name of the on-premises instance to deregister.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"instanceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-deregister-on-premises-instance-input-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: DeregisterOnPremisesInstanceInput
---
