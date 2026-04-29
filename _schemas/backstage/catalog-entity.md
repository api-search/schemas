---
description: A Backstage catalog entity.
layout: schema
name: Entity
properties_list:
- description: The API version of the entity schema.
  name: apiVersion
  type: string
- description: The kind of entity. Common kinds include Component, API, System, Domain, Resource, Group, User, Location, and Template.
  name: kind
  type: string
- description: ''
  name: metadata
  type: object
- description: The specification of the entity. The schema varies depending on the kind and type.
  name: spec
  type: object
- description: ''
  name: relations
  type: array
- description: ''
  name: status
  type: object
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/catalog-entity-schema.json
slug: catalog-entity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/catalog-entity-schema.json\",\n  \"title\": \"Entity\",\n  \"description\": \"A Backstage catalog entity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The API version of the entity schema.\",\n      \"example\": \"backstage.io/v1alpha1\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The kind of entity. Common kinds include Component, API, System, Domain, Resource, Group, User, Location, and Template.\",\n      \"example\": \"Component\"\n    },\n    \"metadata\": {\n      \"$ref\": \"#/components/schemas/EntityMetadata\"\n    },\n    \"spec\": {\n      \"type\": \"object\",\n      \"description\": \"The specification of the entity. The schema varies depending on the kind and type.\",\n      \"\
  additionalProperties\": true\n    },\n    \"relations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/EntityRelation\"\n      }\n    },\n    \"status\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"items\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\"\n              },\n              \"level\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"info\",\n                  \"warning\",\n                  \"error\"\n                ]\n              },\n              \"message\": {\n                \"type\": \"string\"\n              },\n              \"error\": {\n                \"type\": \"object\"\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"apiVersion\",\n    \"kind\",\n    \"metadata\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/catalog-entity-schema.json
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: Entity
---
