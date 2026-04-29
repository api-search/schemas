---
description: UpdateFindingsFeedbackRequest schema from Amazon GuardDuty API
layout: schema
name: UpdateFindingsFeedbackRequest
properties_list:
- description: ''
  name: FindingIds
  type: object
- description: ''
  name: Feedback
  type: object
- description: ''
  name: Comments
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-update-findings-feedback-request-schema.json
slug: guardduty-update-findings-feedback-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-update-findings-feedback-request-schema.json\",\n  \"title\": \"UpdateFindingsFeedbackRequest\",\n  \"description\": \"UpdateFindingsFeedbackRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FindingIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingIds\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"findingIds\"\n          },\n          \"description\": \"The IDs of the findings that you want to mark as useful or not useful.\"\n        }\n      ]\n    },\n    \"Feedback\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Feedback\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"feedback\"\n          },\n          \"description\": \"\
  The feedback for the finding.\"\n        }\n      ]\n    },\n    \"Comments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"comments\"\n          },\n          \"description\": \"Additional feedback about the GuardDuty findings.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FindingIds\",\n    \"Feedback\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-update-findings-feedback-request-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: UpdateFindingsFeedbackRequest
---
