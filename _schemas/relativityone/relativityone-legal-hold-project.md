---
description: A legal hold project in RelativityOne for managing litigation holds and eDiscovery workflows.
layout: schema
name: Legal Hold Project
properties_list:
- description: The unique artifact ID of the legal hold project.
  name: artifactId
  type: integer
- description: The name of the legal hold project.
  name: name
  type: string
- description: The current status of the legal hold project.
  name: status
  type: string
- description: Email address of the project owner.
  name: ownerEmailAddress
  type: string
- description: Optional description of the legal hold project.
  name: description
  type: string
- description: The date the project was created.
  name: createdDate
  type: string
- description: The date the project was last modified.
  name: modifiedDate
  type: string
provider_name: RelativityOne
provider_slug: relativityone
schema_file: json-schema/relativityone-legal-hold-project-schema.json
slug: relativityone-legal-hold-project
source_filename: relativityone-legal-hold-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/relativityone/main/json-schema/relativityone-legal-hold-project-schema.json\",\n  \"title\": \"Legal Hold Project\",\n  \"description\": \"A legal hold project in RelativityOne for managing litigation holds and eDiscovery workflows.\",\n  \"type\": \"object\",\n  \"required\": [\"artifactId\", \"name\", \"status\"],\n  \"properties\": {\n    \"artifactId\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique artifact ID of the legal hold project.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the legal hold project.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the legal hold project.\",\n      \"enum\": [\"Active\", \"Closed\", \"Draft\"]\n    },\n    \"ownerEmailAddress\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the project owner.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the legal hold project.\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date the project was created.\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date the project was last modified.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/relativityone/refs/heads/main/json-schema/relativityone-legal-hold-project-schema.json
tags:
- eDiscovery
- Legal
- Legal Hold
- Document Management
- Compliance
- Litigation
title: Legal Hold Project
---
