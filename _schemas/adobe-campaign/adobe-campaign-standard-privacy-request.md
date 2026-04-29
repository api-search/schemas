---
description: PrivacyRequest from Adobe Campaign API
layout: schema
name: PrivacyRequest
properties_list:
- description: Name identifying the privacy request.
  name: name
  type: string
- description: The namespace name used to identify the data subject (e.g., email, phone).
  name: namespaceName
  type: string
- description: The value used to look up the data subject in the specified namespace (e.g., the email address).
  name: reconciliationValue
  type: string
- description: The privacy regulation for the request.
  name: regulation
  type: string
- description: Whether to access or delete the data subject data.
  name: type
  type: string
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-standard-privacy-request-schema.json
slug: adobe-campaign-standard-privacy-request
source_filename: adobe-campaign-standard-privacy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-privacy-request-schema.json\",\n  \"title\": \"PrivacyRequest\",\n  \"description\": \"PrivacyRequest from Adobe Campaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name identifying the privacy request.\",\n      \"example\": \"Example Campaign\"\n    },\n    \"namespaceName\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace name used to identify the data subject (e.g., email, phone).\",\n      \"example\": \"Example Campaign\"\n    },\n    \"reconciliationValue\": {\n      \"type\": \"string\",\n      \"description\": \"The value used to look up the data subject in the specified namespace (e.g., the email address).\",\n      \"example\": \"example_value\"\n    },\n    \"regulation\"\
  : {\n      \"type\": \"string\",\n      \"enum\": [\n        \"gdpr\",\n        \"ccpa\"\n      ],\n      \"description\": \"The privacy regulation for the request.\",\n      \"example\": \"gdpr\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"access\",\n        \"delete\"\n      ],\n      \"description\": \"Whether to access or delete the data subject data.\",\n      \"example\": \"access\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"namespaceName\",\n    \"reconciliationValue\",\n    \"regulation\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-privacy-request-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: PrivacyRequest
---
