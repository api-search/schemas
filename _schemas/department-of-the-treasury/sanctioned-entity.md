---
description: An individual, entity, vessel, or aircraft listed on an OFAC sanctions list.
layout: schema
name: Sanctioned Entity
properties_list:
- description: ''
  name: uid
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: programs
  type: array
- description: ''
  name: sanctionsListType
  type: string
- description: ''
  name: akas
  type: array
- description: ''
  name: addresses
  type: array
- description: ''
  name: ids
  type: array
- description: ''
  name: nationalities
  type: array
provider_name: Department of the Treasury
provider_slug: department-of-the-treasury
schema_file: json-schema/sanctioned-entity-schema.json
slug: sanctioned-entity
source_filename: sanctioned-entity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/department-of-the-treasury/schemas/sanctioned-entity.json\",\n  \"title\": \"Sanctioned Entity\",\n  \"description\": \"An individual, entity, vessel, or aircraft listed on an OFAC sanctions list.\",\n  \"type\": \"object\",\n  \"required\": [\"uid\", \"name\", \"type\"],\n  \"properties\": {\n    \"uid\": { \"type\": \"string\" },\n    \"name\": { \"type\": \"string\" },\n    \"type\": { \"type\": \"string\", \"enum\": [\"Individual\", \"Entity\", \"Aircraft\", \"Vessel\"] },\n    \"programs\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n    \"sanctionsListType\": { \"type\": \"string\", \"enum\": [\"SDN\", \"Consolidated\"] },\n    \"akas\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"category\": { \"type\": \"string\" },\n          \"type\": { \"type\": \"string\" },\n\
  \          \"firstName\": { \"type\": [\"string\", \"null\"] },\n          \"lastName\": { \"type\": [\"string\", \"null\"] }\n        }\n      }\n    },\n    \"addresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"address1\": { \"type\": [\"string\", \"null\"] },\n          \"city\": { \"type\": [\"string\", \"null\"] },\n          \"stateOrProvince\": { \"type\": [\"string\", \"null\"] },\n          \"postalCode\": { \"type\": [\"string\", \"null\"] },\n          \"country\": { \"type\": [\"string\", \"null\"] }\n        }\n      }\n    },\n    \"ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": { \"type\": \"string\" },\n          \"number\": { \"type\": \"string\" },\n          \"country\": { \"type\": [\"string\", \"null\"] }\n        }\n      }\n    },\n    \"nationalities\": { \"type\": \"array\", \"items\": { \"type\"\
  : \"string\" } }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/department-of-the-treasury/refs/heads/main/json-schema/sanctioned-entity-schema.json
tags:
- Federal Government
- Finance
- Debt
- Sanctions
title: Sanctioned Entity
---
