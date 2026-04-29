---
description: The <code>UpdatePipelineNotificationsRequest</code> structure.
layout: schema
name: UpdatePipelineNotificationsRequest
properties_list:
- description: ''
  name: Notifications
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-update-pipeline-notifications-request-schema.json
slug: amazon-elastic-transcoder-update-pipeline-notifications-request
source_filename: amazon-elastic-transcoder-update-pipeline-notifications-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-update-pipeline-notifications-request-schema.json\",\n  \"title\": \"UpdatePipelineNotificationsRequest\",\n  \"description\": \"The <code>UpdatePipelineNotificationsRequest</code> structure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Notifications\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Notifications\"\n        },\n        {\n          \"description\": \"<p>The topic ARN for the Amazon Simple Notification Service (Amazon SNS) topic that you want to notify to report job status.</p> <important> <p>To receive notifications, you must also subscribe to the new topic in the Amazon SNS console.</p> </important> <ul> <li> <p> <b>Progressing</b>: The topic ARN for the Amazon Simple Notification Service (Amazon SNS) topic that\
  \ you want to notify when Elastic Transcoder has started to process jobs that are added to this pipeline. This is the ARN that Amazon SNS returned when you created the topic.</p> </li> <li> <p> <b>Complete</b>: The topic ARN for the Amazon SNS topic that you want to notify when Elastic Transcoder has finished processing a job. This is the ARN that Amazon SNS returned when you created the topic.</p> </li> <li> <p> <b>Warning</b>: The topic ARN for the Amazon SNS topic that you want to notify when Elastic Transcoder encounters a warning condition. This is the ARN that Amazon SNS returned when you created the topic.</p> </li> <li> <p> <b>Error</b>: The topic ARN for the Amazon SNS topic that you want to notify when Elastic Transcoder encounters an error condition. This is the ARN that Amazon SNS returned when you created the topic.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Notifications\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-update-pipeline-notifications-request-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: UpdatePipelineNotificationsRequest
---
