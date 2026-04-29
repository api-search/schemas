---
description: OrganizationAcl from LinkedIn API
layout: schema
name: OrganizationAcl
properties_list:
- description: Organization URN
  name: organization
  type: string
- description: Role in the organization
  name: role
  type: string
- description: State of the role assignment
  name: state
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-campaigns-organization-acl-schema.json
slug: linkedin-marketing-campaigns-organization-acl
source_filename: linkedin-marketing-campaigns-organization-acl-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-organization-acl-schema.json\",\n  \"title\": \"OrganizationAcl\",\n  \"description\": \"OrganizationAcl from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"organization\": {\n      \"type\": \"string\",\n      \"description\": \"Organization URN\",\n      \"example\": \"urn:li:organization:12345678\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ADMINISTRATOR\",\n        \"DIRECT_SPONSORED_CONTENT_POSTER\",\n        \"RECRUITING_POSTER\",\n        \"LEAD_GEN_FORMS_MANAGER\"\n      ],\n      \"description\": \"Role in the organization\",\n      \"example\": \"ADMINISTRATOR\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"APPROVED\",\n        \"REVOKED\",\n        \"REQUESTED\"\n     \
  \ ],\n      \"description\": \"State of the role assignment\",\n      \"example\": \"APPROVED\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-organization-acl-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: OrganizationAcl
---
