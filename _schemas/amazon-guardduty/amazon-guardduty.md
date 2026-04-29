---
description: Represents an Amazon GuardDuty security finding with its associated details, severity, and metadata.
layout: schema
name: Amazon GuardDuty Finding
properties_list:
- description: The unique identifier of the finding
  name: id
  type: string
- description: The AWS account ID where the finding was generated
  name: accountId
  type: string
- description: The AWS Region where the finding was generated
  name: region
  type: string
- description: The type of finding (e.g., UnauthorizedAccess:EC2/MaliciousIPCaller)
  name: type
  type: string
- description: The severity of the finding (0.0 to 10.0)
  name: severity
  type: number
- description: The title of the finding
  name: title
  type: string
- description: The description of the finding
  name: description
  type: string
- description: The confidence level of the finding
  name: confidence
  type: number
- description: The resource affected by the finding
  name: resource
  type: object
- description: Additional information about the finding
  name: service
  type: object
- description: The time the finding was first observed
  name: createdAt
  type: string
- description: The time the finding was last updated
  name: updatedAt
  type: string
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/amazon-guardduty-schema.json
slug: amazon-guardduty
source_filename: amazon-guardduty-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/amazon/guardduty/finding.json\",\n  \"title\": \"Amazon GuardDuty Finding\",\n  \"description\": \"Represents an Amazon GuardDuty security finding with its associated details, severity, and metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"type\", \"severity\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the finding\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS account ID where the finding was generated\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS Region where the finding was generated\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of finding (e.g., UnauthorizedAccess:EC2/MaliciousIPCaller)\"\n    },\n    \"severity\": {\n      \"type\"\
  : \"number\",\n      \"description\": \"The severity of the finding (0.0 to 10.0)\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the finding\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the finding\"\n    },\n    \"confidence\": {\n      \"type\": \"number\",\n      \"description\": \"The confidence level of the finding\"\n    },\n    \"resource\": {\n      \"type\": \"object\",\n      \"description\": \"The resource affected by the finding\",\n      \"properties\": {\n        \"resourceType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of AWS resource\"\n        },\n        \"instanceDetails\": {\n          \"type\": \"object\",\n          \"description\": \"Details about the EC2 instance involved\"\n        },\n        \"accessKeyDetails\": {\n          \"type\": \"object\",\n          \"description\": \"Details about the IAM access key involved\"\
  \n        }\n      }\n    },\n    \"service\": {\n      \"type\": \"object\",\n      \"description\": \"Additional information about the finding\",\n      \"properties\": {\n        \"action\": {\n          \"type\": \"object\",\n          \"description\": \"Information about the activity\"\n        },\n        \"count\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of times this finding was observed\"\n        },\n        \"detectorId\": {\n          \"type\": \"string\",\n          \"description\": \"The detector ID that generated the finding\"\n        }\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the finding was first observed\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the finding was last updated\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/amazon-guardduty-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: Amazon GuardDuty Finding
---
