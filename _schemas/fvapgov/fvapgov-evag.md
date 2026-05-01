---
description: JSON Schema representation of the FVAP electronic Voting Assistance Guide (eVAG) feed combining important info, deadline dates, ballot rules, and election offices.
layout: schema
name: FVAP eVAG
properties_list:
- description: ''
  name: important-info
  type: object
- description: ''
  name: deadline-dates
  type: array
- description: ''
  name: ballot-rules
  type: object
- description: ''
  name: election-offices
  type: array
provider_name: FVAP.gov
provider_slug: fvapgov
schema_file: json-schema/fvapgov-evag-schema.json
slug: fvapgov-evag
source_filename: fvapgov-evag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/fvapgov/refs/heads/main/json-schema/fvapgov-evag-schema.json\",\n  \"title\": \"FVAP eVAG\",\n  \"description\": \"JSON Schema representation of the FVAP electronic Voting Assistance Guide (eVAG) feed combining important info, deadline dates, ballot rules, and election offices.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"important-info\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"questions\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"question\": { \"type\": \"string\" },\n              \"answer\": { \"type\": \"string\" }\n            }\n          }\n        }\n      }\n    },\n    \"deadline-dates\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n  \
  \        \"election-type\": { \"type\": \"string\" },\n          \"voting-request-type\": { \"type\": \"string\" },\n          \"voter-type\": { \"type\": \"string\" },\n          \"location\": { \"type\": \"string\" },\n          \"date\": { \"type\": [\"string\", \"null\"], \"format\": \"date\" }\n        }\n      }\n    },\n    \"ballot-rules\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"fpca\": { \"$ref\": \"#/$defs/ruleList\" },\n        \"fwab\": { \"$ref\": \"#/$defs/ruleList\" },\n        \"vbr\":  { \"$ref\": \"#/$defs/ruleList\" }\n      }\n    },\n    \"election-offices\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"jurisdiction\":      { \"type\": \"string\" },\n          \"jurisdiction-type\": { \"type\": \"string\" },\n          \"fax\":               { \"type\": \"string\" },\n          \"email\":             { \"type\": \"string\", \"format\": \"email\" },\n          \"\
  street\":            { \"type\": \"string\" },\n          \"city\":              { \"type\": \"string\" },\n          \"state\":             { \"type\": \"string\" },\n          \"zip\":               { \"type\": \"string\" }\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"ruleList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"label\":        { \"type\": \"string\" },\n          \"instructions\": { \"type\": \"string\" }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fvapgov/refs/heads/main/json-schema/fvapgov-evag-schema.json
tags:
- Government
- Voting
title: FVAP eVAG
---
