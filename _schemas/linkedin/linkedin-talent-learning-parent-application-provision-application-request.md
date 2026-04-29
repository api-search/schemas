---
description: Request body for provisioning a new child application
layout: schema
name: ProvisionApplicationRequest
properties_list:
- description: Name of the customer application
  name: name
  type: string
- description: Description of the application
  name: description
  type: string
- description: Unique identifier for the customer in the partner's system
  name: uniqueForeignId
  type: string
- description: List of authorized OAuth 2.0 callback URLs
  name: oauth2AuthorizedCallbackUrls
  type: array
- description: List of valid JavaScript SDK domains
  name: validJsSdkDomains
  type: array
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-learning-parent-application-provision-application-request-schema.json
slug: linkedin-talent-learning-parent-application-provision-application-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-learning-parent-application-provision-application-request-schema.json\",\n  \"title\": \"ProvisionApplicationRequest\",\n  \"description\": \"Request body for provisioning a new child application\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the customer application\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the application\",\n      \"example\": \"Test application for Acme Corporation\"\n    },\n    \"uniqueForeignId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the customer in the partner's system\",\n      \"example\": \"acme-corp-12345\"\n    },\n    \"oauth2AuthorizedCallbackUrls\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"List of authorized OAuth 2.0 callback URLs\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      },\n      \"example\": [\n        \"https://app.acme.com/oauth2/callback\",\n        \"https://staging.acme.com/oauth2/callback\"\n      ]\n    },\n    \"validJsSdkDomains\": {\n      \"type\": \"array\",\n      \"description\": \"List of valid JavaScript SDK domains\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"https://app.acme.com\",\n        \"http://localhost:5000\"\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"uniqueForeignId\",\n    \"oauth2AuthorizedCallbackUrls\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-learning-parent-application-provision-application-request-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: ProvisionApplicationRequest
---
