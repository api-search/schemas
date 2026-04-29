---
description: Contains information about CloudTrail access.
layout: schema
name: CloudTrailProperties
properties_list:
- description: ''
  name: trailProperties
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: endTime
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-cloud-trail-properties-schema.json
slug: iam-access-analyzer-cloud-trail-properties
source_filename: iam-access-analyzer-cloud-trail-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-cloud-trail-properties-schema.json\",\n  \"title\": \"CloudTrailProperties\",\n  \"description\": \"Contains information about CloudTrail access.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"trailProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrailPropertiesList\"\n        },\n        {\n          \"description\": \"A <code>TrailProperties</code> object that contains settings for trail properties.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The start of the time range for which IAM Access Analyzer reviews your CloudTrail events. Events with a timestamp before this time are\
  \ not considered to generate a policy.\"\n        }\n      ]\n    },\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The end of the time range for which IAM Access Analyzer reviews your CloudTrail events. Events with a timestamp after this time are not considered to generate a policy. If this is not included in the request, the default value is the current time.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"trailProperties\",\n    \"startTime\",\n    \"endTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-cloud-trail-properties-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: CloudTrailProperties
---
