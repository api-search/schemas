---
description: Represents the input of a <code>ListOnPremisesInstances</code> operation.
layout: schema
name: ListOnPremisesInstancesInput
properties_list:
- description: ''
  name: registrationStatus
  type: object
- description: ''
  name: tagFilters
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-list-on-premises-instances-input-schema.json
slug: amazon-codedeploy-list-on-premises-instances-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-on-premises-instances-input-schema.json\",\n  \"title\": \"ListOnPremisesInstancesInput\",\n  \"description\": \"Represents the input of a <code>ListOnPremisesInstances</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"registrationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistrationStatus\"\n        },\n        {\n          \"description\": \"<p>The registration status of the on-premises instances:</p> <ul> <li> <p> <code>Deregistered</code>: Include deregistered on-premises instances in the resulting list.</p> </li> <li> <p> <code>Registered</code>: Include registered on-premises instances in the resulting list.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"tagFilters\": {\n      \"allOf\": [\n     \
  \   {\n          \"$ref\": \"#/components/schemas/TagFilterList\"\n        },\n        {\n          \"description\": \"The on-premises instance tags that are used to restrict the on-premises instance names returned.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"An identifier returned from the previous list on-premises instances call. It can be used to return the next set of on-premises instances in the list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-on-premises-instances-input-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: ListOnPremisesInstancesInput
---
