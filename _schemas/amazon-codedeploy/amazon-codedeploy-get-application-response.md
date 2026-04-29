---
description: GetApplicationResponse schema from Amazon CodeDeploy
layout: schema
name: GetApplicationResponse
properties_list:
- description: ''
  name: application
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-get-application-response-schema.json
slug: amazon-codedeploy-get-application-response
source_filename: amazon-codedeploy-get-application-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-application-response-schema.json\",\n  \"title\": \"GetApplicationResponse\",\n  \"description\": \"GetApplicationResponse schema from Amazon CodeDeploy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"application\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"applicationId\": {\n          \"type\": \"string\"\n        },\n        \"applicationName\": {\n          \"type\": \"string\"\n        },\n        \"computePlatform\": {\n          \"type\": \"string\"\n        },\n        \"createTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"linkedToGitHub\": {\n          \"type\": \"boolean\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-application-response-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: GetApplicationResponse
---
