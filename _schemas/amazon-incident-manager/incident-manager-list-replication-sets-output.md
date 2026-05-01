---
description: ListReplicationSetsOutput schema
layout: schema
name: ListReplicationSetsOutput
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: replicationSetArns
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-list-replication-sets-output-schema.json
slug: incident-manager-list-replication-sets-output
source_filename: incident-manager-list-replication-sets-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-list-replication-sets-output-schema.json\",\n  \"title\": \"ListReplicationSetsOutput\",\n  \"description\": \"ListReplicationSetsOutput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The pagination token to continue to the next page of results.\"\n        }\n      ]\n    },\n    \"replicationSetArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReplicationSetArnList\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the list replication set.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"replicationSetArns\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-list-replication-sets-output-schema.json
tags:
- Automation
- DevOps
- Incident Management
- Operations
title: ListReplicationSetsOutput
---
