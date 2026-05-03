---
description: A custodian assigned to a legal hold project in RelativityOne, representing an individual whose data is subject to preservation.
layout: schema
name: Legal Hold Custodian
properties_list:
- description: The unique artifact ID of the custodian.
  name: artifactId
  type: integer
- description: First name of the custodian.
  name: firstName
  type: string
- description: Last name of the custodian.
  name: lastName
  type: string
- description: Email address of the custodian.
  name: emailAddress
  type: string
- description: Optional employee identifier from the HR system.
  name: employeeId
  type: string
- description: Current hold status of the custodian.
  name: status
  type: string
provider_name: RelativityOne
provider_slug: relativityone
schema_file: json-schema/relativityone-custodian-schema.json
slug: relativityone-custodian
source_filename: relativityone-custodian-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/relativityone/main/json-schema/relativityone-custodian-schema.json\",\n  \"title\": \"Legal Hold Custodian\",\n  \"description\": \"A custodian assigned to a legal hold project in RelativityOne, representing an individual whose data is subject to preservation.\",\n  \"type\": \"object\",\n  \"required\": [\"artifactId\", \"emailAddress\"],\n  \"properties\": {\n    \"artifactId\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique artifact ID of the custodian.\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name of the custodian.\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the custodian.\"\n    },\n    \"emailAddress\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the custodian.\"\
  \n    },\n    \"employeeId\": {\n      \"type\": \"string\",\n      \"description\": \"Optional employee identifier from the HR system.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current hold status of the custodian.\",\n      \"enum\": [\"Active\", \"Released\", \"Pending\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/relativityone/refs/heads/main/json-schema/relativityone-custodian-schema.json
tags:
- eDiscovery
- Legal
- Legal Hold
- Document Management
- Compliance
- Litigation
title: Legal Hold Custodian
---
