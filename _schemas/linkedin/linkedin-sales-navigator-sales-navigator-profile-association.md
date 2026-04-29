---
description: SalesNavigatorProfileAssociation from LinkedIn API
layout: schema
name: SalesNavigatorProfileAssociation
properties_list:
- description: LinkedIn Person URN
  name: member
  type: string
- description: Absolute URL of the Sales Navigator profile
  name: profile
  type: string
- description: Absolute URL of the LinkedIn profile photo (optional)
  name: profilePhoto
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-sales-navigator-sales-navigator-profile-association-schema.json
slug: linkedin-sales-navigator-sales-navigator-profile-association
source_filename: linkedin-sales-navigator-sales-navigator-profile-association-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-sales-navigator-sales-navigator-profile-association-schema.json\",\n  \"title\": \"SalesNavigatorProfileAssociation\",\n  \"description\": \"SalesNavigatorProfileAssociation from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"member\": {\n      \"type\": \"string\",\n      \"description\": \"LinkedIn Person URN\",\n      \"example\": \"urn:li:person:ABC123def\"\n    },\n    \"profile\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Absolute URL of the Sales Navigator profile\",\n      \"example\": \"https://www.linkedin.com/sales/people/ABC123def\"\n    },\n    \"profilePhoto\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Absolute URL of the LinkedIn profile photo (optional)\",\n      \"example\": \"\
  https://media.licdn.com/dms/image/ABC123/profile.jpg\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-sales-navigator-sales-navigator-profile-association-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: SalesNavigatorProfileAssociation
---
