---
description: Contains a cluster's state, a cluster's ID, and other important information.
layout: schema
name: ClusterListEntry
properties_list:
- description: ''
  name: ClusterId
  type: object
- description: ''
  name: ClusterState
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: Description
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-cluster-list-entry-schema.json
slug: amazon-snow-family-cluster-list-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-cluster-list-entry-schema.json\",\n  \"title\": \"ClusterListEntry\",\n  \"description\": \"Contains a cluster's state, a cluster's ID, and other important information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The 39-character ID for the cluster that you want to list, for example <code>CID123e4567-e89b-12d3-a456-426655440000</code>.\"\n        }\n      ]\n    },\n    \"ClusterState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClusterState\"\n        },\n        {\n          \"description\": \"The current state of this cluster. For information about the state of a specific node, see\
  \ <a>JobListEntry$JobState</a>.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The creation date for this cluster.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Defines an optional description of the cluster, for example <code>Environmental Data Cluster-01</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-cluster-list-entry-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: ClusterListEntry
---
