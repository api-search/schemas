---
description: JSON Schema for a RescueGroups.org adoptable animal record as returned by the v5 API.
layout: schema
name: RescueGroups.org Animal
properties_list:
- description: Unique animal identifier.
  name: id
  type: string
- description: JSON API resource type.
  name: type
  type: string
- description: ''
  name: attributes
  type: object
- description: ''
  name: relationships
  type: object
provider_name: RescueGroups.org
provider_slug: rescuegroups-org
schema_file: json-schema/rescuegroups-org-animal-schema.json
slug: rescuegroups-org-animal
source_filename: rescuegroups-org-animal-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/rescuegroups-org/json-schema/rescuegroups-org-animal-schema.json\",\n  \"title\": \"RescueGroups.org Animal\",\n  \"description\": \"JSON Schema for a RescueGroups.org adoptable animal record as returned by the v5 API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique animal identifier.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"animals\",\n      \"description\": \"JSON API resource type.\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Animal name.\"\n        },\n        \"birthDate\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\",\n          \"description\": \"Animal birth date.\"\n        },\n    \
  \    \"sex\": {\n          \"type\": \"string\",\n          \"enum\": [\"Male\", \"Female\", \"Unknown\"],\n          \"description\": \"Animal sex.\"\n        },\n        \"ageGroup\": {\n          \"type\": \"string\",\n          \"enum\": [\"Baby\", \"Young\", \"Adult\", \"Senior\"],\n          \"description\": \"Age group category.\"\n        },\n        \"sizeGroup\": {\n          \"type\": \"string\",\n          \"enum\": [\"Small\", \"Medium\", \"Large\", \"Extra Large\"],\n          \"description\": \"Size group category.\"\n        },\n        \"isAdoptionPending\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether adoption is pending.\"\n        },\n        \"isAltered\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the animal is spayed or neutered.\"\n        },\n        \"pictureCount\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of pictures available.\"\n        },\n\
  \        \"videoCount\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of videos available.\"\n        },\n        \"adoptedDate\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\",\n          \"description\": \"Date the animal was adopted.\"\n        },\n        \"specialNeedsDetails\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Description of any special needs.\"\n        },\n        \"descriptionText\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Plain text description of the animal.\"\n        },\n        \"locationCitystate\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"City and state where the animal is located.\"\n        },\n        \"locationState\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"State where the animal is located.\"\n        },\n        \"locationDistance\"\
  : {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Distance from search location.\"\n        },\n        \"rescueId\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"External rescue ID.\"\n        },\n        \"url\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"description\": \"URL of the animal profile page.\"\n        }\n      }\n    },\n    \"relationships\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"breeds\": {\n          \"type\": \"object\",\n          \"description\": \"Animal breed relationships.\"\n        },\n        \"colors\": {\n          \"type\": \"object\",\n          \"description\": \"Animal color relationships.\"\n        },\n        \"patterns\": {\n          \"type\": \"object\",\n          \"description\": \"Animal pattern relationships.\"\n        },\n        \"species\": {\n          \"type\": \"object\",\n          \"description\":\
  \ \"Animal species relationship.\"\n        },\n        \"orgs\": {\n          \"type\": \"object\",\n          \"description\": \"Rescue organization relationship.\"\n        },\n        \"pictures\": {\n          \"type\": \"object\",\n          \"description\": \"Animal pictures relationship.\"\n        }\n      }\n    }\n  },\n  \"required\": [\"id\", \"type\", \"attributes\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rescuegroups-org/refs/heads/main/json-schema/rescuegroups-org-animal-schema.json
tags:
- Animals
- Pet Adoption
- Rescue
- Animal Welfare
title: RescueGroups.org Animal
---
