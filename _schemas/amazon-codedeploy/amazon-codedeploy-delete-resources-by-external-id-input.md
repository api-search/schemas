---
description: DeleteResourcesByExternalIdInput schema from Amazon CodeDeploy
layout: schema
name: DeleteResourcesByExternalIdInput
properties_list:
- description: ''
  name: externalId
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-delete-resources-by-external-id-input-schema.json
slug: amazon-codedeploy-delete-resources-by-external-id-input
source_filename: amazon-codedeploy-delete-resources-by-external-id-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-delete-resources-by-external-id-input-schema.json\",\n  \"title\": \"DeleteResourcesByExternalIdInput\",\n  \"description\": \"DeleteResourcesByExternalIdInput schema from Amazon CodeDeploy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"externalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalId\"\n        },\n        {\n          \"description\": \"The unique ID of an external resource (for example, a CloudFormation stack ID) that is linked to one or more CodeDeploy resources.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-delete-resources-by-external-id-input-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: DeleteResourcesByExternalIdInput
---
