---
description: An autofill job for generating designs from brand templates
layout: schema
name: AutofillJob
properties_list:
- description: The autofill job ID
  name: id
  type: string
- description: The current status of the autofill job
  name: status
  type: string
- description: The autofill result (present when status is success)
  name: result
  type: object
- description: Error details (present when status is failed)
  name: error
  type: object
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-autofill-job-schema.json
slug: canva-connect-autofill-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AutofillJob\",\n  \"type\": \"object\",\n  \"description\": \"An autofill job for generating designs from brand templates\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The autofill job ID\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the autofill job\"\n    },\n    \"result\": {\n      \"type\": \"object\",\n      \"description\": \"The autofill result (present when status is success)\"\n    },\n    \"error\": {\n      \"type\": \"object\",\n      \"description\": \"Error details (present when status is failed)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-autofill-job-schema.json
tags:
- Apps
- Automation
- Brand Management
- Collaboration
- Design
- Graphics
- Marketing
- Print
- Templates
- Visual Content
title: AutofillJob
---
