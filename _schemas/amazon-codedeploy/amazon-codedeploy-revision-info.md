---
description: Information about an application revision.
layout: schema
name: RevisionInfo
properties_list:
- description: ''
  name: revisionLocation
  type: object
- description: ''
  name: genericRevisionInfo
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-revision-info-schema.json
slug: amazon-codedeploy-revision-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-revision-info-schema.json\",\n  \"title\": \"RevisionInfo\",\n  \"description\": \"Information about an application revision.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"revisionLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionLocation\"\n        },\n        {\n          \"description\": \"Information about the location and type of an application revision.\"\n        }\n      ]\n    },\n    \"genericRevisionInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericRevisionInfo\"\n        },\n        {\n          \"description\": \"Information about an application revision, including usage details and associated deployment groups.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-revision-info-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: RevisionInfo
---
