---
description: Schema for an Apache Software Foundation Incubator podling as returned by the Projects and Whimsy APIs.
layout: schema
name: Apache Software Foundation Podling
properties_list:
- description: The podling display name
  name: name
  type: string
- description: Current incubation status of the podling
  name: status
  type: string
- description: A brief description of the podling
  name: description
  type: string
- description: The podling homepage URL
  name: homepage
  type: string
- description: Date the podling entered incubation
  name: startdate
  type: string
- description: Date the podling left incubation (graduated or retired)
  name: enddate
  type: string
- description: The sponsoring PMC or Incubator
  name: sponsor
  type: string
- description: Apache ID of the podling champion
  name: champion
  type: string
- description: List of mentor Apache IDs
  name: mentors
  type: array
- description: Resolution details if the podling graduated or retired
  name: resolution
  type: string
provider_name: Apache Software Foundation
provider_slug: apache-software-foundation
schema_file: json-schema/apache-software-foundation-podling-schema.json
slug: apache-software-foundation-podling
source_filename: apache-software-foundation-podling-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"apache-software-foundation-podling-schema.json\",\n  \"title\": \"Apache Software Foundation Podling\",\n  \"description\": \"Schema for an Apache Software Foundation Incubator podling as returned by the Projects and Whimsy APIs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The podling display name\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"current\", \"graduated\", \"retired\"],\n      \"description\": \"Current incubation status of the podling\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A brief description of the podling\"\n    },\n    \"homepage\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The podling homepage URL\"\n    },\n    \"startdate\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Date the podling entered incubation\"\n    },\n    \"enddate\": {\n      \"type\": \"string\",\n      \"description\": \"Date the podling left incubation (graduated or retired)\"\n    },\n    \"sponsor\": {\n      \"type\": \"string\",\n      \"description\": \"The sponsoring PMC or Incubator\"\n    },\n    \"champion\": {\n      \"type\": \"string\",\n      \"description\": \"Apache ID of the podling champion\"\n    },\n    \"mentors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of mentor Apache IDs\"\n    },\n    \"resolution\": {\n      \"type\": \"string\",\n      \"description\": \"Resolution details if the podling graduated or retired\"\n    }\n  },\n  \"required\": [\"name\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-software-foundation/refs/heads/main/json-schema/apache-software-foundation-podling-schema.json
tags:
- ASF
- Open Source
- Governance
- Projects
- Apache
title: Apache Software Foundation Podling
---
