---
description: ''
layout: schema
name: BetaTesterAttributes
properties_list:
- description: The first name of the beta tester
  name: firstName
  type: '[''string'', ''null'']'
- description: The last name of the beta tester
  name: lastName
  type: '[''string'', ''null'']'
- description: The email address of the beta tester
  name: email
  type: '[''string'', ''null'']'
- description: How the tester was invited
  name: inviteType
  type: string
- description: The current state of the beta tester invitation
  name: state
  type: string
provider_name: Apple
provider_slug: apple
schema_file: json-schema/app-store-connect-beta-tester-attributes-schema.json
slug: app-store-connect-beta-tester-attributes
source_filename: app-store-connect-beta-tester-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BetaTesterAttributes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"firstName\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The first name of the beta tester\"\n    },\n    \"lastName\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The last name of the beta tester\"\n    },\n    \"email\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The email address of the beta tester\"\n    },\n    \"inviteType\": {\n      \"type\": \"string\",\n      \"description\": \"How the tester was invited\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the beta tester invitation\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apple/refs/heads/main/json-schema/app-store-connect-beta-tester-attributes-schema.json
tags:
- Developer
- iOS
- macOS
- Mobile
- Technology
title: BetaTesterAttributes
---
