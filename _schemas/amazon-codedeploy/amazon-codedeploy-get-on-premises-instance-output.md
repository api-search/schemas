---
description: Represents the output of a <code>GetOnPremisesInstance</code> operation.
layout: schema
name: GetOnPremisesInstanceOutput
properties_list:
- description: ''
  name: instanceInfo
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-get-on-premises-instance-output-schema.json
slug: amazon-codedeploy-get-on-premises-instance-output
source_filename: amazon-codedeploy-get-on-premises-instance-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-on-premises-instance-output-schema.json\",\n  \"title\": \"GetOnPremisesInstanceOutput\",\n  \"description\": \" Represents the output of a <code>GetOnPremisesInstance</code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceInfo\"\n        },\n        {\n          \"description\": \" Information about the on-premises instance. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-on-premises-instance-output-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: GetOnPremisesInstanceOutput
---
