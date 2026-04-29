---
description: Summary of the AWS resource used for access control that is implicitly linked to your AWS account.
layout: schema
name: ProgressUpdateStreamSummary
properties_list:
- description: ''
  name: ProgressUpdateStreamName
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-progress-update-stream-summary-schema.json
slug: migration-hub-api-progress-update-stream-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-progress-update-stream-summary-schema.json\",\n  \"title\": \"ProgressUpdateStreamSummary\",\n  \"description\": \"Summary of the AWS resource used for access control that is implicitly linked to your AWS account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProgressUpdateStreamName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProgressUpdateStream\"\n        },\n        {\n          \"description\": \"The name of the ProgressUpdateStream. <i>Do not store personal data in this field.</i> \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-progress-update-stream-summary-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ProgressUpdateStreamSummary
---
