---
description: Schema representing a customer profile in the Optimizely Data Platform (ODP), including identity resolution, attributes, computed insights, and segment membership.
layout: schema
name: Optimizely Customer Profile
properties_list:
- description: Customer identifiers used for identity resolution across channels
  name: identifiers
  type: object
- description: Customer profile attributes
  name: attributes
  type: object
- description: Computed customer intelligence and behavioral insights
  name: insights
  type: object
- description: List of segment names the customer belongs to
  name: segments
  type: array
- description: Recent events associated with this customer
  name: events
  type: array
provider_name: Optimizely
provider_slug: optimizely
schema_file: json-schema/optimizely-customer-profile-schema.json
slug: optimizely-customer-profile
source_filename: optimizely-customer-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.optimizely.com/schemas/optimizely/customer-profile.json\",\n  \"title\": \"Optimizely Customer Profile\",\n  \"description\": \"Schema representing a customer profile in the Optimizely Data Platform (ODP), including identity resolution, attributes, computed insights, and segment membership.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identifiers\": {\n      \"type\": \"object\",\n      \"description\": \"Customer identifiers used for identity resolution across channels\",\n      \"properties\": {\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Customer email address\"\n        },\n        \"customer_id\": {\n          \"type\": \"string\",\n          \"description\": \"External customer identifier from source systems\"\n        },\n        \"vuid\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Visitor unique identifier assigned by ODP tracking\",\n          \"pattern\": \"^[a-f0-9-]+$\"\n        }\n      }\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Customer profile attributes\",\n      \"properties\": {\n        \"first_name\": {\n          \"type\": \"string\",\n          \"description\": \"Customer first name\",\n          \"maxLength\": 255\n        },\n        \"last_name\": {\n          \"type\": \"string\",\n          \"description\": \"Customer last name\",\n          \"maxLength\": 255\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"Customer city\",\n          \"maxLength\": 255\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"Customer state or province\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"Customer country\",\n          \"maxLength\": 2,\n          \"pattern\": \"\
  ^[A-Z]{2}$\"\n        },\n        \"zip_code\": {\n          \"type\": \"string\",\n          \"description\": \"Customer postal code\",\n          \"maxLength\": 20\n        },\n        \"phone\": {\n          \"type\": \"string\",\n          \"description\": \"Customer phone number\"\n        },\n        \"date_of_birth\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Customer date of birth\"\n        },\n        \"gender\": {\n          \"type\": \"string\",\n          \"description\": \"Customer gender\"\n        }\n      }\n    },\n    \"insights\": {\n      \"type\": \"object\",\n      \"description\": \"Computed customer intelligence and behavioral insights\",\n      \"properties\": {\n        \"total_revenue\": {\n          \"type\": \"number\",\n          \"description\": \"Total lifetime revenue from this customer\"\n        },\n        \"order_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Total\
  \ number of orders placed\",\n          \"minimum\": 0\n        },\n        \"average_order_value\": {\n          \"type\": \"number\",\n          \"description\": \"Average order value across all purchases\"\n        },\n        \"first_order_date\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Date of the customer's first order\"\n        },\n        \"last_order_date\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Date of the customer's most recent order\"\n        },\n        \"engagement_score\": {\n          \"type\": \"number\",\n          \"description\": \"Computed engagement score based on activity\"\n        }\n      }\n    },\n    \"segments\": {\n      \"type\": \"array\",\n      \"description\": \"List of segment names the customer belongs to\",\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"Segment identifier\"\n      }\n   \
  \ },\n    \"events\": {\n      \"type\": \"array\",\n      \"description\": \"Recent events associated with this customer\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CustomerEvent\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"CustomerEvent\": {\n      \"type\": \"object\",\n      \"description\": \"An event associated with a customer in ODP\",\n      \"required\": [\"type\", \"action\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Event type category (e.g., order, product, email, navigation)\"\n        },\n        \"action\": {\n          \"type\": \"string\",\n          \"description\": \"Specific action within the event type (e.g., purchase, view, open)\"\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the event occurred\"\n        },\n        \"data\": {\n          \"type\": \"object\",\n          \"description\": \"\
  Additional event data fields\",\n          \"additionalProperties\": true\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/json-schema/optimizely-customer-profile-schema.json
tags:
- A/B Testing
- Content Management
- Customer Data
- E-Commerce
- Experimentation
- Feature Flags
- Marketing
title: Optimizely Customer Profile
---
