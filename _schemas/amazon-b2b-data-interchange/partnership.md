---
description: Represents a B2B Data Interchange partnership — a connection between a customer profile and a trading partner with associated EDI capabilities.
layout: schema
name: Partnership
properties_list:
- description: Unique identifier for the partnership
  name: partnershipId
  type: string
- description: Amazon Resource Name (ARN) for the partnership
  name: partnershipArn
  type: string
- description: Identifier of the profile associated with this partnership
  name: profileId
  type: string
- description: Name of the partnership
  name: name
  type: string
- description: Email address of the trading partner contact
  name: email
  type: string
- description: Phone number of the trading partner contact
  name: phone
  type: string
- description: List of capability IDs associated with this partnership
  name: capabilities
  type: array
- description: Identifier assigned to the trading partner
  name: tradingPartnerId
  type: string
- description: Timestamp when the partnership was created
  name: createdAt
  type: string
- description: Timestamp when the partnership was last modified
  name: modifiedAt
  type: string
provider_name: Amazon B2B Data Interchange
provider_slug: amazon-b2b-data-interchange
schema_file: json-schema/partnership.json
slug: partnership
source_filename: partnership.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/main/json-schema/partnership.json\",\n  \"title\": \"Partnership\",\n  \"description\": \"Represents a B2B Data Interchange partnership — a connection between a customer profile and a trading partner with associated EDI capabilities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"partnershipId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the partnership\",\n      \"pattern\": \"^ps-[a-zA-Z0-9]+$\"\n    },\n    \"partnershipArn\": {\n      \"type\": \"string\",\n      \"description\": \"Amazon Resource Name (ARN) for the partnership\"\n    },\n    \"profileId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the profile associated with this partnership\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the partnership\"\
  ,\n      \"minLength\": 1,\n      \"maxLength\": 254\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the trading partner contact\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number of the trading partner contact\"\n    },\n    \"capabilities\": {\n      \"type\": \"array\",\n      \"description\": \"List of capability IDs associated with this partnership\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"minItems\": 1\n    },\n    \"tradingPartnerId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier assigned to the trading partner\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the partnership was created\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when\
  \ the partnership was last modified\"\n    }\n  },\n  \"required\": [\"partnershipId\", \"partnershipArn\", \"profileId\", \"name\", \"email\", \"capabilities\", \"createdAt\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/refs/heads/main/json-schema/partnership.json
tags:
- EDI
- B2B
- Data Interchange
- Supply Chain
- Healthcare
- Financial Services
- Amazon Web Services
title: Partnership
---
