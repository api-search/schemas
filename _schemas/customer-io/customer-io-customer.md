---
description: A customer profile in Customer.io representing a person in your audience with attributes, device information, and segment membership.
layout: schema
name: Customer.io Customer
properties_list:
- description: ''
  name: identifiers
  type: object
- description: The customer email address used for email messaging.
  name: email
  type: string
- description: A UNIX timestamp representing when the customer was first identified.
  name: created_at
  type: integer
- description: An anonymous identifier used to associate pre-identification events with this customer.
  name: anonymous_id
  type: string
- description: Custom attributes on the customer profile. These can be any key-value pairs set via the Track or Pipelines APIs.
  name: attributes
  type: object
- description: Whether the customer has unsubscribed from marketing messages.
  name: unsubscribed
  type: boolean
- description: Push notification devices associated with this customer.
  name: devices
  type: array
- description: Segments the customer belongs to.
  name: segments
  type: array
provider_name: Customer.io
provider_slug: customer-io
schema_file: json-schema/customer-io-customer-schema.json
slug: customer-io-customer
source_filename: customer-io-customer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://customer.io/schemas/customer-io/customer.json\",\n  \"title\": \"Customer.io Customer\",\n  \"description\": \"A customer profile in Customer.io representing a person in your audience with attributes, device information, and segment membership.\",\n  \"type\": \"object\",\n  \"required\": [\"identifiers\"],\n  \"properties\": {\n    \"identifiers\": {\n      \"$ref\": \"#/$defs/CustomerIdentifiers\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The customer email address used for email messaging.\"\n    },\n    \"created_at\": {\n      \"type\": \"integer\",\n      \"description\": \"A UNIX timestamp representing when the customer was first identified.\"\n    },\n    \"anonymous_id\": {\n      \"type\": \"string\",\n      \"description\": \"An anonymous identifier used to associate pre-identification events with this customer.\"\
  \n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Custom attributes on the customer profile. These can be any key-value pairs set via the Track or Pipelines APIs.\",\n      \"additionalProperties\": true\n    },\n    \"unsubscribed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the customer has unsubscribed from marketing messages.\"\n    },\n    \"devices\": {\n      \"type\": \"array\",\n      \"description\": \"Push notification devices associated with this customer.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Device\"\n      }\n    },\n    \"segments\": {\n      \"type\": \"array\",\n      \"description\": \"Segments the customer belongs to.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/SegmentMembership\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"CustomerIdentifiers\": {\n      \"type\": \"object\",\n      \"description\": \"Identifiers used to uniquely reference a customer in Customer.io.\",\n      \"properties\"\
  : {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The primary customer identifier in your system.\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The customer email address, which can serve as a primary identifier.\"\n        },\n        \"cio_id\": {\n          \"type\": \"string\",\n          \"description\": \"The Customer.io internal identifier automatically assigned to each customer.\",\n          \"pattern\": \"^[0-9a-f]+$\"\n        }\n      }\n    },\n    \"Device\": {\n      \"type\": \"object\",\n      \"description\": \"A push notification device associated with a customer.\",\n      \"required\": [\"id\", \"platform\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique device token.\"\n        },\n        \"platform\": {\n          \"type\": \"string\",\n          \"description\": \"The device\
  \ platform.\",\n          \"enum\": [\"ios\", \"android\"]\n        },\n        \"last_used\": {\n          \"type\": \"integer\",\n          \"description\": \"A UNIX timestamp of when the device was last used.\"\n        }\n      }\n    },\n    \"SegmentMembership\": {\n      \"type\": \"object\",\n      \"description\": \"A segment that the customer belongs to.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The segment identifier.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The segment name.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/customer-io/refs/heads/main/json-schema/customer-io-customer-schema.json
tags:
- Behavioral Data
- Broadcasts
- Campaigns
- CDP
- Customer Data
- Customer Data Platform
- Data Ingestion
- Email
- Event Tracking
- Marketing Automation
- Messaging
- Push Notifications
- Segments
- SMS
- Transactional Email
title: Customer.io Customer
---
