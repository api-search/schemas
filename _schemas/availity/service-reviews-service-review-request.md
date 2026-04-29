---
description: ServiceReviewRequest schema from Availity API
layout: schema
name: ServiceReviewRequest
properties_list:
- description: ''
  name: payerId
  type: string
- description: ''
  name: requestType
  type: string
- description: ''
  name: provider
  type: object
- description: ''
  name: subscriber
  type: object
- description: ''
  name: serviceInformation
  type: object
provider_name: availity
provider_slug: availity
schema_file: json-schema/service-reviews-service-review-request-schema.json
slug: service-reviews-service-review-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/service-reviews-service-review-request-schema.json\",\n  \"title\": \"ServiceReviewRequest\",\n  \"description\": \"ServiceReviewRequest schema from Availity API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"payerId\",\n    \"provider\",\n    \"subscriber\",\n    \"requestType\"\n  ],\n  \"properties\": {\n    \"payerId\": {\n      \"type\": \"string\",\n      \"example\": \"BCBS001\"\n    },\n    \"requestType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"INITIAL\",\n        \"UPDATE\",\n        \"CANCEL\",\n        \"REFERRAL\"\n      ],\n      \"example\": \"INITIAL\"\n    },\n    \"provider\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"npi\": {\n          \"type\": \"string\",\n          \"example\": \"1234567890\"\n        },\n        \"taxId\": {\n     \
  \     \"type\": \"string\",\n          \"example\": \"123456789\"\n        }\n      }\n    },\n    \"subscriber\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"memberId\": {\n          \"type\": \"string\",\n          \"example\": \"MEM123456\"\n        },\n        \"firstName\": {\n          \"type\": \"string\",\n          \"example\": \"Jane\"\n        },\n        \"lastName\": {\n          \"type\": \"string\",\n          \"example\": \"Smith\"\n        }\n      }\n    },\n    \"serviceInformation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"procedureCodes\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"diagnosisCodes\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"serviceFromDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"\
  serviceToDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/service-reviews-service-review-request-schema.json
tags: []
title: ServiceReviewRequest
---
