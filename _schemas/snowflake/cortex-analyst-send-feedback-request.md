---
description: The request object for sending user feedback on Cortex Analyst responses
layout: schema
name: SendFeedbackRequest
properties_list:
- description: Request id associated with the feedback
  name: request_id
  type: string
- description: Whether the response was good (true) or bad (false)
  name: positive
  type: boolean
- description: The text for the detailed feedback message
  name: feedback_message
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-analyst-send-feedback-request-schema.json
slug: cortex-analyst-send-feedback-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SendFeedbackRequest\",\n  \"type\": \"object\",\n  \"description\": \"The request object for sending user feedback on Cortex Analyst responses\",\n  \"properties\": {\n    \"request_id\": {\n      \"type\": \"string\",\n      \"description\": \"Request id associated with the feedback\"\n    },\n    \"positive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the response was good (true) or bad (false)\"\n    },\n    \"feedback_message\": {\n      \"type\": \"string\",\n      \"description\": \"The text for the detailed feedback message\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-analyst-send-feedback-request-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: SendFeedbackRequest
---
