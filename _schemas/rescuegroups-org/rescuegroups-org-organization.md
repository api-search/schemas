---
description: JSON Schema for a RescueGroups.org rescue organization record.
layout: schema
name: RescueGroups.org Organization
properties_list:
- description: Unique organization identifier.
  name: id
  type: string
- description: JSON API resource type.
  name: type
  type: string
- description: ''
  name: attributes
  type: object
provider_name: RescueGroups.org
provider_slug: rescuegroups-org
schema_file: json-schema/rescuegroups-org-organization-schema.json
slug: rescuegroups-org-organization
source_filename: rescuegroups-org-organization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/rescuegroups-org/json-schema/rescuegroups-org-organization-schema.json\",\n  \"title\": \"RescueGroups.org Organization\",\n  \"description\": \"JSON Schema for a RescueGroups.org rescue organization record.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique organization identifier.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"orgs\",\n      \"description\": \"JSON API resource type.\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Organization name.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Organization type (rescue, shelter, etc.).\"\n        },\n        \"email\": {\n          \"\
  type\": [\"string\", \"null\"],\n          \"format\": \"email\",\n          \"description\": \"Contact email address.\"\n        },\n        \"phone\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Contact phone number.\"\n        },\n        \"street\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Street address.\"\n        },\n        \"city\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"City.\"\n        },\n        \"state\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"State or province.\"\n        },\n        \"country\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Country.\"\n        },\n        \"postalcode\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Postal code.\"\n        },\n        \"url\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"\
  description\": \"Organization website URL.\"\n        },\n        \"adoptionUrl\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"description\": \"Adoption application URL.\"\n        },\n        \"about\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Organization description.\"\n        },\n        \"serveAreas\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Geographic areas the organization serves.\"\n        },\n        \"facebookUrl\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"description\": \"Facebook page URL.\"\n        }\n      },\n      \"required\": [\"name\"]\n    }\n  },\n  \"required\": [\"id\", \"type\", \"attributes\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rescuegroups-org/refs/heads/main/json-schema/rescuegroups-org-organization-schema.json
tags:
- Animals
- Pet Adoption
- Rescue
- Animal Welfare
title: RescueGroups.org Organization
---
