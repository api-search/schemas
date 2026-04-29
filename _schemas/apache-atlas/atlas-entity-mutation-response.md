---
description: Response from entity create, update, or delete operations.
layout: schema
name: EntityMutationResponse
properties_list:
- description: Map of client-side temporary GUIDs to server-assigned GUIDs.
  name: guidAssignments
  type: object
- description: Map of mutation type (CREATE, UPDATE, DELETE) to list of mutated entity headers.
  name: mutatedEntities
  type: object
provider_name: Apache Atlas
provider_slug: apache-atlas
schema_file: json-schema/atlas-entity-mutation-response-schema.json
slug: atlas-entity-mutation-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-entity-mutation-response-schema.json\",\n  \"title\": \"EntityMutationResponse\",\n  \"description\": \"Response from entity create, update, or delete operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"guidAssignments\": {\n      \"type\": \"object\",\n      \"description\": \"Map of client-side temporary GUIDs to server-assigned GUIDs.\",\n      \"example\": {\n        \"-1\": \"a1b2c3d4-e5f6-7890-abcd-ef1234567890\"\n      }\n    },\n    \"mutatedEntities\": {\n      \"type\": \"object\",\n      \"description\": \"Map of mutation type (CREATE, UPDATE, DELETE) to list of mutated entity headers.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-entity-mutation-response-schema.json
tags:
- Apache
- Big Data
- Compliance
- Data Governance
- Data Lineage
- Hadoop
- Metadata
- Open Source
title: EntityMutationResponse
---
