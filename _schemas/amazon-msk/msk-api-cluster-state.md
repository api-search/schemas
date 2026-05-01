---
description: <p>The state of the Apache Kafka cluster.</p>
layout: schema
name: ClusterState
properties_list: []
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-cluster-state-schema.json
slug: msk-api-cluster-state
source_filename: msk-api-cluster-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-cluster-state-schema.json\",\n  \"title\": \"ClusterState\",\n  \"description\": \"\\n            <p>The state of the Apache Kafka cluster.</p>\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ACTIVE\",\n    \"CREATING\",\n    \"DELETING\",\n    \"FAILED\",\n    \"HEALING\",\n    \"MAINTENANCE\",\n    \"REBOOTING_BROKER\",\n    \"UPDATING\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-cluster-state-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ClusterState
---
