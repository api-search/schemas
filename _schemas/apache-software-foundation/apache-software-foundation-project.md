---
description: Schema for an Apache Software Foundation top-level project as returned by the Projects API.
layout: schema
name: Apache Software Foundation Project
properties_list:
- description: The official project name
  name: name
  type: string
- description: The project category (e.g., big-data, cloud, library)
  name: category
  type: string
- description: The Project Management Committee responsible for this project
  name: pmc
  type: string
- description: A brief description of the project
  name: description
  type: string
- description: The project homepage URL
  name: homepage
  type: string
- description: Primary programming language used by the project
  name: programming-language
  type: string
- description: URL of the project bug tracker
  name: bug-database
  type: string
- description: URL of the project downloads page
  name: download-page
  type: string
- description: URL of the project mailing list archives
  name: mailing-list
  type: string
- description: Source code repository URLs
  name: repository
  type: array
- description: The software license (typically Apache-2.0)
  name: license
  type: string
- description: A short one-line description of the project
  name: shortdesc
  type: string
provider_name: Apache Software Foundation
provider_slug: apache-software-foundation
schema_file: json-schema/apache-software-foundation-project-schema.json
slug: apache-software-foundation-project
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"apache-software-foundation-project-schema.json\",\n  \"title\": \"Apache Software Foundation Project\",\n  \"description\": \"Schema for an Apache Software Foundation top-level project as returned by the Projects API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The official project name\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The project category (e.g., big-data, cloud, library)\"\n    },\n    \"pmc\": {\n      \"type\": \"string\",\n      \"description\": \"The Project Management Committee responsible for this project\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A brief description of the project\"\n    },\n    \"homepage\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The project homepage\
  \ URL\"\n    },\n    \"programming-language\": {\n      \"type\": \"string\",\n      \"description\": \"Primary programming language used by the project\"\n    },\n    \"bug-database\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the project bug tracker\"\n    },\n    \"download-page\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the project downloads page\"\n    },\n    \"mailing-list\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the project mailing list archives\"\n    },\n    \"repository\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      },\n      \"description\": \"Source code repository URLs\"\n    },\n    \"license\": {\n      \"type\": \"string\",\n      \"description\": \"The software license (typically Apache-2.0)\"\n    },\n    \"shortdesc\": {\n      \"type\": \"\
  string\",\n      \"description\": \"A short one-line description of the project\"\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-software-foundation/refs/heads/main/json-schema/apache-software-foundation-project-schema.json
tags:
- ASF
- Open Source
- Governance
- Projects
- Apache
title: Apache Software Foundation Project
---
