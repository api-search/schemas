---
description: Helix partition state assignment across instances
layout: schema
name: Partition
properties_list:
- description: Partition name
  name: id
  type: string
- description: Map of instance to state
  name: instanceStateMap
  type: object
provider_name: Apache Helix
provider_slug: apache-helix
schema_file: json-schema/helix-rest-partition-schema.json
slug: helix-rest-partition
source_filename: helix-rest-partition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-helix/json-schema/helix-rest-partition-schema.json\",\n  \"title\": \"Partition\",\n  \"type\": \"object\",\n  \"description\": \"Helix partition state assignment across instances\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Partition name\",\n      \"example\": \"my-resource_0\"\n    },\n    \"instanceStateMap\": {\n      \"type\": \"object\",\n      \"description\": \"Map of instance to state\",\n      \"example\": {\n        \"localhost_12913\": \"MASTER\",\n        \"localhost_12914\": \"SLAVE\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-helix/refs/heads/main/json-schema/helix-rest-partition-schema.json
tags:
- Apache
- Cluster Management
- Distributed Systems
- Open Source
- Partitioning
- Replication
title: Partition
---
