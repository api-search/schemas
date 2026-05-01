---
description: Represents the output of a <code>StopDeployment</code> operation.
layout: schema
name: StopDeploymentOutput
properties_list:
- description: ''
  name: status
  type: object
- description: ''
  name: statusMessage
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-stop-deployment-output-schema.json
slug: amazon-codedeploy-stop-deployment-output
source_filename: amazon-codedeploy-stop-deployment-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-stop-deployment-output-schema.json\",\n  \"title\": \"StopDeploymentOutput\",\n  \"description\": \" Represents the output of a <code>StopDeployment</code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StopStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the stop deployment operation:</p> <ul> <li> <p>Pending: The stop operation is pending.</p> </li> <li> <p>Succeeded: The stop operation was successful.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"statusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"An accompanying status message.\"\n \
  \       }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-stop-deployment-output-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: StopDeploymentOutput
---
