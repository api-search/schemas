---
description: OrgUnit from Adobe Campaign API
layout: schema
name: OrgUnit
properties_list:
- description: Unique identifier for the organizational unit.
  name: PKey
  type: string
- description: Internal name of the organizational unit.
  name: name
  type: string
- description: Display label of the organizational unit.
  name: label
  type: string
- description: Label of the parent organizational unit.
  name: parentTitle
  type: string
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-standard-org-unit-schema.json
slug: adobe-campaign-standard-org-unit
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-org-unit-schema.json\",\n  \"title\": \"OrgUnit\",\n  \"description\": \"OrgUnit from Adobe Campaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PKey\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the organizational unit.\",\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Internal name of the organizational unit.\",\n      \"example\": \"Example Campaign\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Display label of the organizational unit.\",\n      \"example\": \"Example Campaign\"\n    },\n    \"parentTitle\": {\n      \"type\": \"string\",\n      \"description\": \"Label of the parent organizational unit.\",\n      \"example\"\
  : \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-org-unit-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: OrgUnit
---
