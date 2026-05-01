---
description: Information about an application.
layout: schema
name: ApplicationInfo
properties_list:
- description: ''
  name: applicationId
  type: object
- description: ''
  name: applicationName
  type: object
- description: ''
  name: createTime
  type: object
- description: ''
  name: linkedToGitHub
  type: object
- description: ''
  name: gitHubAccountName
  type: object
- description: ''
  name: computePlatform
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-application-info-schema.json
slug: amazon-codedeploy-application-info
source_filename: amazon-codedeploy-application-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-application-info-schema.json\",\n  \"title\": \"ApplicationInfo\",\n  \"description\": \"Information about an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationId\"\n        },\n        {\n          \"description\": \"The application ID.\"\n        }\n      ]\n    },\n    \"applicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The application name.\"\n        }\n      ]\n    },\n    \"createTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at\
  \ which the application was created.\"\n        }\n      ]\n    },\n    \"linkedToGitHub\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"True if the user has authenticated with GitHub for the specified application. Otherwise, false.\"\n        }\n      ]\n    },\n    \"gitHubAccountName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GitHubAccountTokenName\"\n        },\n        {\n          \"description\": \"The name for a connection to a GitHub account.\"\n        }\n      ]\n    },\n    \"computePlatform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputePlatform\"\n        },\n        {\n          \"description\": \"The destination platform type for deployment of the application (<code>Lambda</code> or <code>Server</code>).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-application-info-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: ApplicationInfo
---
