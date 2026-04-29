---
description: Response containing provisioned application details
layout: schema
name: ProvisionApplicationResponse
properties_list:
- description: URN of the provisioned application
  name: applicationUrn
  type: string
- description: OAuth 2.0 client ID for the application
  name: clientId
  type: string
- description: OAuth 2.0 client secret for the application
  name: clientSecret
  type: string
- description: Name of the application
  name: name
  type: string
- description: Partner's unique identifier for the customer
  name: uniqueForeignId
  type: string
- description: ''
  name: oauth2AuthorizedCallbackUrls
  type: array
- description: ''
  name: validJsSdkDomains
  type: array
- description: Timestamp of application creation
  name: createdAt
  type: integer
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-learning-parent-application-provision-application-response-schema.json
slug: linkedin-talent-learning-parent-application-provision-application-response
source_filename: linkedin-talent-learning-parent-application-provision-application-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-learning-parent-application-provision-application-response-schema.json\",\n  \"title\": \"ProvisionApplicationResponse\",\n  \"description\": \"Response containing provisioned application details\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationUrn\": {\n      \"type\": \"string\",\n      \"description\": \"URN of the provisioned application\",\n      \"example\": \"urn:li:developerApplication:12345678\"\n    },\n    \"clientId\": {\n      \"type\": \"string\",\n      \"description\": \"OAuth 2.0 client ID for the application\",\n      \"example\": \"78abc123def456\"\n    },\n    \"clientSecret\": {\n      \"type\": \"string\",\n      \"description\": \"OAuth 2.0 client secret for the application\",\n      \"example\": \"secretXYZ789\"\n    },\n    \"name\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Name of the application\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"uniqueForeignId\": {\n      \"type\": \"string\",\n      \"description\": \"Partner's unique identifier for the customer\",\n      \"example\": \"acme-corp-12345\"\n    },\n    \"oauth2AuthorizedCallbackUrls\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      },\n      \"example\": [\n        \"https://app.acme.com/oauth2/callback\"\n      ]\n    },\n    \"validJsSdkDomains\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"https://app.acme.com\"\n      ]\n    },\n    \"createdAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Timestamp of application creation\",\n      \"example\": 1702693664000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-learning-parent-application-provision-application-response-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: ProvisionApplicationResponse
---
