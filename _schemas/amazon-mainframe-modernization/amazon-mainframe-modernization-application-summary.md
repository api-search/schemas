---
description: A subset of the possible application attributes. Used in the application list.
layout: schema
name: ApplicationSummary
properties_list:
- description: ''
  name: applicationArn
  type: object
- description: ''
  name: applicationId
  type: object
- description: ''
  name: applicationVersion
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: deploymentStatus
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: engineType
  type: object
- description: ''
  name: environmentId
  type: object
- description: ''
  name: lastStartTime
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: versionStatus
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-application-summary-schema.json
slug: amazon-mainframe-modernization-application-summary
source_filename: amazon-mainframe-modernization-application-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-application-summary-schema.json\",\n  \"title\": \"ApplicationSummary\",\n  \"description\": \"A subset of the possible application attributes. Used in the application list.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the application.\"\n        }\n      ]\n    },\n    \"applicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The unique identifier of the application.\"\n        }\n      ]\n    },\n    \"applicationVersion\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"The version of the application.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp when the application was created.\"\n        }\n      ]\n    },\n    \"deploymentStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationDeploymentLifecycle\"\n        },\n        {\n          \"description\": \"Indicates either an ongoing deployment or if the application has ever deployed successfully.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityDescription\"\n        },\n        {\n          \"description\": \"The description of the application.\"\n        }\n      ]\n    },\n    \"engineType\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/EngineType\"\n        },\n        {\n          \"description\": \"The type of the target platform for this application.\"\n        }\n      ]\n    },\n    \"environmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The unique identifier of the runtime environment that hosts this application.\"\n        }\n      ]\n    },\n    \"lastStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp when you last started the application. Null until the application runs for the first time.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityName\"\n        },\n        {\n          \"description\": \"The name of the application.\"\n        }\n      ]\n    },\n\
  \    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the role associated with the application.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationLifecycle\"\n        },\n        {\n          \"description\": \"The status of the application.\"\n        }\n      ]\n    },\n    \"versionStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionLifecycle\"\n        },\n        {\n          \"description\": \"Indicates the status of the latest version of the application.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"applicationArn\",\n    \"applicationId\",\n    \"applicationVersion\",\n    \"creationTime\",\n    \"engineType\",\n    \"name\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-application-summary-schema.json
tags:
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: ApplicationSummary
---
