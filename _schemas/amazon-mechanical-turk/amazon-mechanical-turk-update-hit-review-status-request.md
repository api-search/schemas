---
description: UpdateHITReviewStatusRequest schema from Amazon Mechanical Turk API
layout: schema
name: UpdateHITReviewStatusRequest
properties_list:
- description: ''
  name: HITId
  type: object
- description: ''
  name: Revert
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-update-hit-review-status-request-schema.json
slug: amazon-mechanical-turk-update-hit-review-status-request
source_filename: amazon-mechanical-turk-update-hit-review-status-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-update-hit-review-status-request-schema.json\",\n  \"title\": \"UpdateHITReviewStatusRequest\",\n  \"description\": \"UpdateHITReviewStatusRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HITId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \" The ID of the HIT to update. \"\n        }\n      ]\n    },\n    \"Revert\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p> Specifies how to update the HIT status. Default is <code>False</code>. </p> <ul> <li> <p> Setting this to false will only transition a HIT from <code>Reviewable</code> to\
  \ <code>Reviewing</code> </p> </li> <li> <p> Setting this to true will only transition a HIT from <code>Reviewing</code> to <code>Reviewable</code> </p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"HITId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-update-hit-review-status-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: UpdateHITReviewStatusRequest
---
