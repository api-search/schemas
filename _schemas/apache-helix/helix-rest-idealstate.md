---
description: Desired ideal state for resource partition placement
layout: schema
name: IdealState
properties_list:
- description: Resource name
  name: id
  type: string
- description: State model reference
  name: stateModelDefRef
  type: string
- description: Map of partition to desired instance state map
  name: mapFields
  type: object
provider_name: Apache Helix
provider_slug: apache-helix
schema_file: json-schema/helix-rest-idealstate-schema.json
slug: helix-rest-idealstate
source_filename: helix-rest-idealstate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-helix/json-schema/helix-rest-idealstate-schema.json\",\n  \"title\": \"IdealState\",\n  \"type\": \"object\",\n  \"description\": \"Desired ideal state for resource partition placement\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Resource name\",\n      \"example\": \"my-resource\"\n    },\n    \"stateModelDefRef\": {\n      \"type\": \"string\",\n      \"description\": \"State model reference\",\n      \"example\": \"MasterSlave\"\n    },\n    \"mapFields\": {\n      \"type\": \"object\",\n      \"description\": \"Map of partition to desired instance state map\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-helix/refs/heads/main/json-schema/helix-rest-idealstate-schema.json
tags:
- Apache
- Cluster Management
- Distributed Systems
- Open Source
- Partitioning
- Replication
title: IdealState
---
