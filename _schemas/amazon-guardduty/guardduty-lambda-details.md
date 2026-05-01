---
description: Information about the Lambda function involved in the finding.
layout: schema
name: LambdaDetails
properties_list:
- description: ''
  name: FunctionArn
  type: object
- description: ''
  name: FunctionName
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: LastModifiedAt
  type: object
- description: ''
  name: RevisionId
  type: object
- description: ''
  name: FunctionVersion
  type: object
- description: ''
  name: Role
  type: object
- description: ''
  name: VpcConfig
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-lambda-details-schema.json
slug: guardduty-lambda-details
source_filename: guardduty-lambda-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-lambda-details-schema.json\",\n  \"title\": \"LambdaDetails\",\n  \"description\": \"Information about the Lambda function involved in the finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FunctionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"functionArn\"\n          },\n          \"description\": \"Amazon Resource Name (ARN) of the Lambda function.\"\n        }\n      ]\n    },\n    \"FunctionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"functionName\"\n          },\n          \"description\": \"Name of the Lambda function.\"\n        }\n      ]\n\
  \    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"Description of the Lambda function.\"\n        }\n      ]\n    },\n    \"LastModifiedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"lastModifiedAt\"\n          },\n          \"description\": \"The timestamp when the Lambda function was last modified. This field is in the UTC date string format <code>(2023-03-22T19:37:20.168Z)</code>.\"\n        }\n      ]\n    },\n    \"RevisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"revisionId\"\n          },\n          \"description\": \"The revision ID of the Lambda function\
  \ version.\"\n        }\n      ]\n    },\n    \"FunctionVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"functionVersion\"\n          },\n          \"description\": \"The version of the Lambda function.\"\n        }\n      ]\n    },\n    \"Role\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"role\"\n          },\n          \"description\": \"The execution role of the Lambda function.\"\n        }\n      ]\n    },\n    \"VpcConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcConfig\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vpcConfig\"\n          },\n          \"description\": \"Amazon Virtual Private Cloud configuration details associated with your Lambda function.\"\n        }\n      ]\n    },\n\
  \    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"A list of tags attached to this resource, listed in the format of <code>key</code>:<code>value</code> pair.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-lambda-details-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: LambdaDetails
---
