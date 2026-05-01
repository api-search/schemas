---
description: Object representing the on-premises resource being migrated.
layout: schema
name: DiscoveredResource
properties_list:
- description: ''
  name: ConfigurationId
  type: object
- description: ''
  name: Description
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-discovered-resource-schema.json
slug: migration-hub-api-discovered-resource
source_filename: migration-hub-api-discovered-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-discovered-resource-schema.json\",\n  \"title\": \"DiscoveredResource\",\n  \"description\": \"Object representing the on-premises resource being migrated.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationId\"\n        },\n        {\n          \"description\": \"The configurationId in Application Discovery Service that uniquely identifies the on-premise resource.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DiscoveredResourceDescription\"\n        },\n        {\n          \"description\": \"A description that can be free-form text to record additional detail about the discovered resource\
  \ for clarity or later reference.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigurationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-discovered-resource-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: DiscoveredResource
---
