---
description: restart partitions configuration.
layout: schema
name: RestartZonePartitionsRequest
properties_list:
- description: Names specifying nodes to restart zone partitions. Case-sensitive. If empty/omitted, partitions on all nodes are restarted.
  name: nodeNames
  type: array
- description: Name of the zone to restart partitions of. Without quotes, case-sensitive.
  name: zoneName
  type: string
- description: IDs of partitions to restart. If empty/omitted, all partitions will be restarted.
  name: partitionIds
  type: array
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-restart-zone-partitions-request-schema.json
slug: rest-api-restart-zone-partitions-request
source_filename: rest-api-restart-zone-partitions-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-restart-zone-partitions-request-schema.json\",\n  \"title\": \"RestartZonePartitionsRequest\",\n  \"description\": \"restart partitions configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nodeNames\": {\n      \"type\": \"array\",\n      \"description\": \"Names specifying nodes to restart zone partitions. Case-sensitive. If empty/omitted, partitions on all nodes are restarted.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"zoneName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the zone to restart partitions of. Without quotes, case-sensitive.\"\n    },\n    \"partitionIds\": {\n      \"type\": \"array\",\n      \"description\": \"IDs of partitions to restart. If empty/omitted, all partitions will be restarted.\",\n      \"items\"\
  : {\n        \"type\": \"integer\",\n        \"format\": \"int32\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-restart-zone-partitions-request-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: RestartZonePartitionsRequest
---
