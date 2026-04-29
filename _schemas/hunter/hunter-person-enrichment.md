---
description: ''
layout: schema
name: PersonEnrichment
properties_list:
- description: Unique identifier for the person record.
  name: id
  type: string
- description: ''
  name: name
  type: object
- description: Email address.
  name: email
  type: string
- description: Location description.
  name: location
  type: '[''string'', ''null'']'
- description: Time zone name.
  name: timeZone
  type: '[''string'', ''null'']'
- description: UTC offset in hours.
  name: utcOffset
  type: '[''number'', ''null'']'
- description: Short biography.
  name: bio
  type: '[''string'', ''null'']'
- description: Personal website URL.
  name: site
  type: '[''string'', ''null'']'
- description: Avatar image URL.
  name: avatar
  type: '[''string'', ''null'']'
- description: ''
  name: employment
  type: object
- description: ''
  name: facebook
  type: object
- description: ''
  name: github
  type: object
- description: ''
  name: twitter
  type: object
- description: ''
  name: linkedin
  type: object
- description: Whether the match was fuzzy.
  name: fuzzy
  type: boolean
- description: Email service provider.
  name: emailProvider
  type: '[''string'', ''null'']'
- description: Date when the record was last indexed.
  name: indexedAt
  type: '[''string'', ''null'']'
- description: Phone number.
  name: phone
  type: '[''string'', ''null'']'
- description: Date when the person was last active.
  name: activeAt
  type: '[''string'', ''null'']'
- description: Date when the person became inactive.
  name: inactiveAt
  type: '[''string'', ''null'']'
provider_name: Hunter
provider_slug: hunter
schema_file: json-schema/hunter-person-enrichment-schema.json
slug: hunter-person-enrichment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PersonEnrichment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the person record.\"\n    },\n    \"name\": {\n      \"type\": \"object\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Email address.\"\n    },\n    \"location\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Location description.\"\n    },\n    \"timeZone\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Time zone name.\"\n    },\n    \"utcOffset\": {\n      \"type\": \"['number', 'null']\",\n      \"description\": \"UTC offset in hours.\"\n    },\n    \"bio\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Short biography.\"\n    },\n    \"site\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Personal website URL.\"\
  \n    },\n    \"avatar\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Avatar image URL.\"\n    },\n    \"employment\": {\n      \"type\": \"object\"\n    },\n    \"facebook\": {\n      \"type\": \"object\"\n    },\n    \"github\": {\n      \"type\": \"object\"\n    },\n    \"twitter\": {\n      \"type\": \"object\"\n    },\n    \"linkedin\": {\n      \"type\": \"object\"\n    },\n    \"fuzzy\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the match was fuzzy.\"\n    },\n    \"emailProvider\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Email service provider.\"\n    },\n    \"indexedAt\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Date when the record was last indexed.\"\n    },\n    \"phone\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Phone number.\"\n    },\n    \"activeAt\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Date when the person\
  \ was last active.\"\n    },\n    \"inactiveAt\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Date when the person became inactive.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/json-schema/hunter-person-enrichment-schema.json
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
title: PersonEnrichment
---
