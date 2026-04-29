---
description: CreateReplicationSetOutput schema
layout: schema
name: CreateReplicationSetOutput
properties_list:
- description: ''
  name: arn
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-create-replication-set-output-schema.json
slug: incident-manager-create-replication-set-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-create-replication-set-output-schema.json\",\n  \"title\": \"CreateReplicationSetOutput\",\n  \"description\": \"CreateReplicationSetOutput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the replication set. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-create-replication-set-output-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: CreateReplicationSetOutput
---
