---
description: GetReplicationSetOutput schema
layout: schema
name: GetReplicationSetOutput
properties_list:
- description: ''
  name: replicationSet
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-get-replication-set-output-schema.json
slug: incident-manager-get-replication-set-output
source_filename: incident-manager-get-replication-set-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-get-replication-set-output-schema.json\",\n  \"title\": \"GetReplicationSetOutput\",\n  \"description\": \"GetReplicationSetOutput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"replicationSet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReplicationSet\"\n        },\n        {\n          \"description\": \"Details of the replication set.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"replicationSet\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-get-replication-set-output-schema.json
tags:
- Automation
- DevOps
- Incident Management
- Operations
title: GetReplicationSetOutput
---
