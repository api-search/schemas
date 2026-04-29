---
description: ClusterState schema from Amazon Snow Family API
layout: schema
name: ClusterState
properties_list: []
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-cluster-state-schema.json
slug: amazon-snow-family-cluster-state
source_filename: amazon-snow-family-cluster-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-cluster-state-schema.json\",\n  \"title\": \"ClusterState\",\n  \"description\": \"ClusterState schema from Amazon Snow Family API\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"AwaitingQuorum\",\n    \"Pending\",\n    \"InUse\",\n    \"Complete\",\n    \"Cancelled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-cluster-state-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: ClusterState
---
