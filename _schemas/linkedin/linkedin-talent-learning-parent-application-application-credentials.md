---
description: ApplicationCredentials from LinkedIn API
layout: schema
name: ApplicationCredentials
properties_list:
- description: URN of the application
  name: applicationUrn
  type: string
- description: OAuth 2.0 client ID
  name: clientId
  type: string
- description: OAuth 2.0 client secret
  name: clientSecret
  type: string
- description: Partner's unique identifier
  name: uniqueForeignId
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-learning-parent-application-application-credentials-schema.json
slug: linkedin-talent-learning-parent-application-application-credentials
source_filename: linkedin-talent-learning-parent-application-application-credentials-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-learning-parent-application-application-credentials-schema.json\",\n  \"title\": \"ApplicationCredentials\",\n  \"description\": \"ApplicationCredentials from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationUrn\": {\n      \"type\": \"string\",\n      \"description\": \"URN of the application\",\n      \"example\": \"urn:li:developerApplication:12345678\"\n    },\n    \"clientId\": {\n      \"type\": \"string\",\n      \"description\": \"OAuth 2.0 client ID\",\n      \"example\": \"78abc123def456\"\n    },\n    \"clientSecret\": {\n      \"type\": \"string\",\n      \"description\": \"OAuth 2.0 client secret\",\n      \"example\": \"secretXYZ789\"\n    },\n    \"uniqueForeignId\": {\n      \"type\": \"string\",\n      \"description\": \"Partner's unique identifier\"\
  ,\n      \"example\": \"acme-corp-12345\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-learning-parent-application-application-credentials-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: ApplicationCredentials
---
