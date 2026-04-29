---
description: EntityRelation schema from Backstage catalog API
layout: schema
name: EntityRelation
properties_list:
- description: The type of relation.
  name: type
  type: string
- description: The entity reference of the target entity.
  name: targetRef
  type: string
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/catalog-entity-relation-schema.json
slug: catalog-entity-relation
source_filename: catalog-entity-relation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/catalog-entity-relation-schema.json\",\n  \"title\": \"EntityRelation\",\n  \"description\": \"EntityRelation schema from Backstage catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of relation.\",\n      \"example\": \"ownedBy\"\n    },\n    \"targetRef\": {\n      \"type\": \"string\",\n      \"description\": \"The entity reference of the target entity.\",\n      \"example\": \"group:default/my-team\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/catalog-entity-relation-schema.json
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: EntityRelation
---
