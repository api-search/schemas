---
description: Details used when updating the replication set.
layout: schema
name: UpdateReplicationSetAction
properties_list:
- description: ''
  name: addRegionAction
  type: object
- description: ''
  name: deleteRegionAction
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-update-replication-set-action-schema.json
slug: incident-manager-update-replication-set-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-update-replication-set-action-schema.json\",\n  \"title\": \"UpdateReplicationSetAction\",\n  \"description\": \"Details used when updating the replication set.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"addRegionAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddRegionAction\"\n        },\n        {\n          \"description\": \"Details about the Amazon Web Services Region that you're adding to the replication set.\"\n        }\n      ]\n    },\n    \"deleteRegionAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeleteRegionAction\"\n        },\n        {\n          \"description\": \"Details about the Amazon Web Services Region that you're deleting to the replication set.\"\n        }\n \
  \     ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-update-replication-set-action-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: UpdateReplicationSetAction
---
