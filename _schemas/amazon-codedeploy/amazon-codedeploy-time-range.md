---
description: Information about a time range.
layout: schema
name: TimeRange
properties_list:
- description: ''
  name: start
  type: object
- description: ''
  name: end
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-time-range-schema.json
slug: amazon-codedeploy-time-range
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-time-range-schema.json\",\n  \"title\": \"TimeRange\",\n  \"description\": \"Information about a time range.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"start\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"<p>The start time of the time range.</p> <note> <p>Specify null to leave the start time open-ended.</p> </note>\"\n        }\n      ]\n    },\n    \"end\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"<p>The end time of the time range.</p> <note> <p>Specify null to leave the end time open-ended.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-time-range-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: TimeRange
---
