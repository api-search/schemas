---
description: DescribeApplicationStateResult schema from Amazon Migration Hub API
layout: schema
name: DescribeApplicationStateResult
properties_list:
- description: ''
  name: ApplicationStatus
  type: object
- description: ''
  name: LastUpdatedTime
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-describe-application-state-result-schema.json
slug: migration-hub-api-describe-application-state-result
source_filename: migration-hub-api-describe-application-state-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-describe-application-state-result-schema.json\",\n  \"title\": \"DescribeApplicationStateResult\",\n  \"description\": \"DescribeApplicationStateResult schema from Amazon Migration Hub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationStatus\"\n        },\n        {\n          \"description\": \"Status of the application - Not Started, In-Progress, Complete.\"\n        }\n      ]\n    },\n    \"LastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateDateTime\"\n        },\n        {\n          \"description\": \"The timestamp when the application status was last updated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-describe-application-state-result-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DescribeApplicationStateResult
---
