---
description: Represents the output of the list on-premises instances operation.
layout: schema
name: ListOnPremisesInstancesOutput
properties_list:
- description: ''
  name: instanceNames
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-list-on-premises-instances-output-schema.json
slug: amazon-codedeploy-list-on-premises-instances-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-on-premises-instances-output-schema.json\",\n  \"title\": \"ListOnPremisesInstancesOutput\",\n  \"description\": \"Represents the output of the list on-premises instances operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceNameList\"\n        },\n        {\n          \"description\": \"The list of matching on-premises instance names.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If a large amount of information is returned, an identifier is also returned. It can be used in a subsequent list on-premises instances call to\
  \ return the next set of on-premises instances in the list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-on-premises-instances-output-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: ListOnPremisesInstancesOutput
---
