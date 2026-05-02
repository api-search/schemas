---
description: A Medium publication that aggregates posts from multiple contributors around a shared topic or brand, including its metadata and contributor information.
layout: schema
name: Medium Publication
properties_list:
- description: The unique identifier for the publication.
  name: id
  type: string
- description: The name of the publication as displayed on Medium.
  name: name
  type: string
- description: A short description of the publication's focus or mission.
  name: description
  type: string
- description: The URL to the publication's homepage on Medium.
  name: url
  type: string
- description: The URL to the publication's logo or header image.
  name: imageUrl
  type: string
- description: The list of editors and writers who contribute to the publication.
  name: contributors
  type: array
provider_name: medium
provider_slug: medium
schema_file: json-schema/medium-publication-schema.json
slug: medium-publication
source_filename: medium-publication-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://medium.com/schemas/medium/publication.json\",\n  \"title\": \"Medium Publication\",\n  \"description\": \"A Medium publication that aggregates posts from multiple contributors around a shared topic or brand, including its metadata and contributor information.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the publication.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the publication as displayed on Medium.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A short description of the publication's focus or mission.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to the publication's homepage on Medium.\"\
  \n    },\n    \"imageUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to the publication's logo or header image.\"\n    },\n    \"contributors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Contributor\"\n      },\n      \"description\": \"The list of editors and writers who contribute to the publication.\"\n    }\n  },\n  \"$defs\": {\n    \"Contributor\": {\n      \"type\": \"object\",\n      \"description\": \"A contributor to a Medium publication with a specific editorial role.\",\n      \"required\": [\"userId\", \"role\"],\n      \"properties\": {\n        \"publicationId\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the publication the contributor belongs to.\"\n        },\n        \"userId\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the contributing user.\"\n        },\n        \"role\": {\n       \
  \   \"type\": \"string\",\n          \"enum\": [\"editor\", \"writer\"],\n          \"description\": \"The role of the contributor within the publication. Editors can manage all content while writers can submit drafts.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/medium/refs/heads/main/json-schema/medium-publication-schema.json
tags: []
title: Medium Publication
---
