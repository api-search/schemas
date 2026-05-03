---
description: JSON Schema for a Resend domain object used for email sending configuration.
layout: schema
name: Resend Domain
properties_list:
- description: The ID of the domain.
  name: id
  type: string
- description: The type of object.
  name: object
  type: string
- description: The name of the domain.
  name: name
  type: string
- description: The verification status of the domain.
  name: status
  type: string
- description: The date and time the domain was created.
  name: created_at
  type: string
- description: The region where the domain is hosted.
  name: region
  type: string
- description: DNS records for domain verification.
  name: records
  type: array
provider_name: Resend
provider_slug: resend
schema_file: json-schema/resend-domain-schema.json
slug: resend-domain
source_filename: resend-domain-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/resend/json-schema/resend-domain-schema.json\",\n  \"title\": \"Resend Domain\",\n  \"description\": \"JSON Schema for a Resend domain object used for email sending configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the domain.\",\n      \"example\": \"d91cd9bd-1176-453e-8fc1-35364d380206\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"const\": \"domain\",\n      \"description\": \"The type of object.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the domain.\",\n      \"example\": \"example.com\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The verification status of the domain.\",\n      \"example\": \"not_started\"\n    },\n    \"created_at\": {\n      \"type\": \"\
  string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the domain was created.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"enum\": [\"us-east-1\", \"eu-west-1\", \"sa-east-1\"],\n      \"description\": \"The region where the domain is hosted.\"\n    },\n    \"records\": {\n      \"type\": \"array\",\n      \"description\": \"DNS records for domain verification.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"record\": { \"type\": \"string\" },\n          \"name\": { \"type\": \"string\" },\n          \"type\": { \"type\": \"string\" },\n          \"ttl\": { \"type\": \"string\" },\n          \"status\": { \"type\": \"string\" },\n          \"value\": { \"type\": \"string\" },\n          \"priority\": { \"type\": \"integer\" }\n        }\n      }\n    }\n  },\n  \"required\": [\"id\", \"name\", \"status\", \"created_at\", \"region\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/resend/refs/heads/main/json-schema/resend-domain-schema.json
tags:
- Email
- Developer Tools
- Transactional Email
- Marketing Email
title: Resend Domain
---
