---
description: ComplianceAuthorizationRequest from LinkedIn API
layout: schema
name: ComplianceAuthorizationRequest
properties_list:
- description: URN of the member to regulate
  name: member
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-compliance-events-compliance-authorization-request-schema.json
slug: linkedin-compliance-events-compliance-authorization-request
source_filename: linkedin-compliance-events-compliance-authorization-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-compliance-events-compliance-authorization-request-schema.json\",\n  \"title\": \"ComplianceAuthorizationRequest\",\n  \"description\": \"ComplianceAuthorizationRequest from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"member\": {\n      \"type\": \"string\",\n      \"description\": \"URN of the member to regulate\",\n      \"example\": \"urn:li:person:ABC123def\"\n    }\n  },\n  \"required\": [\n    \"member\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-compliance-events-compliance-authorization-request-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: ComplianceAuthorizationRequest
---
