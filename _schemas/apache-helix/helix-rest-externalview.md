---
description: Current external view showing actual partition states across instances
layout: schema
name: ExternalView
properties_list:
- description: Resource name
  name: id
  type: string
- description: Map of partition to instance state map
  name: mapFields
  type: object
provider_name: Apache Helix
provider_slug: apache-helix
schema_file: json-schema/helix-rest-externalview-schema.json
slug: helix-rest-externalview
source_filename: helix-rest-externalview-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-helix/json-schema/helix-rest-externalview-schema.json\",\n  \"title\": \"ExternalView\",\n  \"type\": \"object\",\n  \"description\": \"Current external view showing actual partition states across instances\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Resource name\",\n      \"example\": \"my-resource\"\n    },\n    \"mapFields\": {\n      \"type\": \"object\",\n      \"description\": \"Map of partition to instance state map\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-helix/refs/heads/main/json-schema/helix-rest-externalview-schema.json
tags:
- Apache
- Cluster Management
- Distributed Systems
- Open Source
- Partitioning
- Replication
title: ExternalView
---
