---
description: UpdateReplicationSetInputActionsList schema
layout: schema
name: UpdateReplicationSetInputActionsList
properties_list: []
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-update-replication-set-input-actions-list-schema.json
slug: incident-manager-update-replication-set-input-actions-list
source_filename: incident-manager-update-replication-set-input-actions-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-update-replication-set-input-actions-list-schema.json\",\n  \"title\": \"UpdateReplicationSetInputActionsList\",\n  \"description\": \"UpdateReplicationSetInputActionsList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"addRegionAction\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AddRegionAction\"\n          },\n          {\n            \"description\": \"Details about the Amazon Web Services Region that you're adding to the replication set.\"\n          }\n        ]\n      },\n      \"deleteRegionAction\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DeleteRegionAction\"\n          },\n          {\n            \"description\": \"Details about\
  \ the Amazon Web Services Region that you're deleting to the replication set.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Details used when updating the replication set.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-update-replication-set-input-actions-list-schema.json
tags:
- Automation
- DevOps
- Incident Management
- Operations
title: UpdateReplicationSetInputActionsList
---
