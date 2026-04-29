---
description: DeliveryAttempt schema from ARGUS Enterprise API
layout: schema
name: DeliveryAttempt
properties_list:
- description: Sequential attempt number
  name: attemptNumber
  type: integer
- description: When the delivery was attempted
  name: timestamp
  type: string
- description: HTTP response status code from the endpoint
  name: responseCode
  type: integer
- description: Response time in milliseconds
  name: responseTime
  type: integer
- description: Whether the delivery was successful
  name: success
  type: boolean
- description: Error message if delivery failed
  name: errorMessage
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-delivery-attempt-schema.json
slug: argus-enterprise-delivery-attempt
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-delivery-attempt-schema.json\",\n  \"title\": \"DeliveryAttempt\",\n  \"description\": \"DeliveryAttempt schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attemptNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Sequential attempt number\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the delivery was attempted\"\n    },\n    \"responseCode\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP response status code from the endpoint\"\n    },\n    \"responseTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Response time in milliseconds\"\n    },\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether\
  \ the delivery was successful\"\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Error message if delivery failed\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-delivery-attempt-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: DeliveryAttempt
---
