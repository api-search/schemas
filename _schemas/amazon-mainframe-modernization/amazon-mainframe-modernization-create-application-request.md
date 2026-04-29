---
description: CreateApplicationRequest schema from AWS Mainframe Modernization API
layout: schema
name: CreateApplicationRequest
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: definition
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: engineType
  type: object
- description: ''
  name: kmsKeyId
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-create-application-request-schema.json
slug: amazon-mainframe-modernization-create-application-request
source_filename: amazon-mainframe-modernization-create-application-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-create-application-request-schema.json\",\n  \"title\": \"CreateApplicationRequest\",\n  \"description\": \"CreateApplicationRequest schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Unique, case-sensitive identifier the service generates to ensure the idempotency of the request to create an application. The service generates the clientToken when the API call is triggered. The token expires after one hour, so if you retry the API within this timeframe with the same clientToken, you will get the same response. The service also handles deleting the clientToken\
  \ after it expires. \"\n        }\n      ]\n    },\n    \"definition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Definition\"\n        },\n        {\n          \"description\": \"The application definition for this application. You can specify either inline JSON or an S3 bucket location.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityDescription\"\n        },\n        {\n          \"description\": \"The description of the application.\"\n        }\n      ]\n    },\n    \"engineType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EngineType\"\n        },\n        {\n          \"description\": \"The type of the target platform for this application.\"\n        }\n      ]\n    },\n    \"kmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"\
  The identifier of a customer managed key.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityName\"\n        },\n        {\n          \"description\": \"The unique identifier of the application.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies a role that the application uses to access Amazon Web Services resources that are not part of the application or are in a different Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A list of tags to apply to the application.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"definition\",\n    \"engineType\",\n    \"name\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-create-application-request-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: CreateApplicationRequest
---
