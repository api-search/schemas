---
description: <p>The Amazon Simple Notification Service (Amazon SNS) topic or topics to notify in order to report job status.</p> <important> <p>To receive notifications, you must also subscribe to the new topic in the Amazon SNS console.</p> </important>
layout: schema
name: Notifications
properties_list:
- description: ''
  name: Progressing
  type: object
- description: ''
  name: Completed
  type: object
- description: ''
  name: Warning
  type: object
- description: ''
  name: Error
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-notifications-schema.json
slug: amazon-elastic-transcoder-notifications
source_filename: amazon-elastic-transcoder-notifications-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-notifications-schema.json\",\n  \"title\": \"Notifications\",\n  \"description\": \"<p>The Amazon Simple Notification Service (Amazon SNS) topic or topics to notify in order to report job status.</p> <important> <p>To receive notifications, you must also subscribe to the new topic in the Amazon SNS console.</p> </important>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Progressing\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnsTopic\"\n        },\n        {\n          \"description\": \"The Amazon Simple Notification Service (Amazon SNS) topic that you want to notify when Elastic Transcoder has started to process the job.\"\n        }\n      ]\n    },\n    \"Completed\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/SnsTopic\"\n        },\n        {\n          \"description\": \"The Amazon SNS topic that you want to notify when Elastic Transcoder has finished processing the job.\"\n        }\n      ]\n    },\n    \"Warning\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnsTopic\"\n        },\n        {\n          \"description\": \"The Amazon SNS topic that you want to notify when Elastic Transcoder encounters a warning condition.\"\n        }\n      ]\n    },\n    \"Error\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnsTopic\"\n        },\n        {\n          \"description\": \"The Amazon SNS topic that you want to notify when Elastic Transcoder encounters an error condition.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-notifications-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: Notifications
---
