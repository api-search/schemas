---
description: Defines the information about the Amazon Web Services Region you're deleting from your replication set.
layout: schema
name: DeleteRegionAction
properties_list:
- description: ''
  name: regionName
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-delete-region-action-schema.json
slug: incident-manager-delete-region-action
source_filename: incident-manager-delete-region-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-delete-region-action-schema.json\",\n  \"title\": \"DeleteRegionAction\",\n  \"description\": \"Defines the information about the Amazon Web Services Region you're deleting from your replication set.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"regionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegionName\"\n        },\n        {\n          \"description\": \"The name of the Amazon Web Services Region you're deleting from the replication set.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"regionName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-delete-region-action-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: DeleteRegionAction
---
