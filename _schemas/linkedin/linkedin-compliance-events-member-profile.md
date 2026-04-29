---
description: MemberProfile from LinkedIn API
layout: schema
name: MemberProfile
properties_list:
- description: First name of the member
  name: firstName
  type: string
- description: Last name of the member
  name: lastName
  type: string
- description: Professional headline
  name: headline
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-compliance-events-member-profile-schema.json
slug: linkedin-compliance-events-member-profile
source_filename: linkedin-compliance-events-member-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-compliance-events-member-profile-schema.json\",\n  \"title\": \"MemberProfile\",\n  \"description\": \"MemberProfile from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name of the member\",\n      \"example\": \"John\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the member\",\n      \"example\": \"Doe\"\n    },\n    \"headline\": {\n      \"type\": \"string\",\n      \"description\": \"Professional headline\",\n      \"example\": \"Software Engineer at Tech Corp\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-compliance-events-member-profile-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: MemberProfile
---
