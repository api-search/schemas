---
description: repositoryParameterAnnouncement schema from Argo CD API
layout: schema
name: repositoryParameterAnnouncement
properties_list:
- description: array is the default value of the parameter if the parameter is an array.
  name: array
  type: array
- description: collectionType is the type of value this parameter holds - either a single value (a string) or a collection (array or map). If collectionType is set, only the field with that type will be used. If col
  name: collectionType
  type: string
- description: itemType determines the primitive data type represented by the parameter. Parameters are always encoded as strings, but this field lets them be interpreted as other primitive types.
  name: itemType
  type: string
- description: map is the default value of the parameter if the parameter is a map.
  name: map
  type: object
- description: name is the name identifying a parameter.
  name: name
  type: string
- description: required defines if this given parameter is mandatory.
  name: required
  type: boolean
- description: string is the default value of the parameter if the parameter is a string.
  name: string
  type: string
- description: title is a human-readable text of the parameter name.
  name: title
  type: string
- description: tooltip is a human-readable description of the parameter.
  name: tooltip
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-repository-parameter-announcement-schema.json
slug: argo-cd-repository-parameter-announcement
source_filename: argo-cd-repository-parameter-announcement-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-parameter-announcement-schema.json\",\n  \"title\": \"repositoryParameterAnnouncement\",\n  \"description\": \"repositoryParameterAnnouncement schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"array\": {\n      \"description\": \"array is the default value of the parameter if the parameter is an array.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"collectionType\": {\n      \"description\": \"collectionType is the type of value this parameter holds - either a single value (a string) or a collection\\n(array or map). If collectionType is set, only the field with that type will be used. If collectionType is not\\nset, `string` is the default. If collectionType is set to an invalid value, a validation error\
  \ is thrown.\",\n      \"type\": \"string\"\n    },\n    \"itemType\": {\n      \"description\": \"itemType determines the primitive data type represented by the parameter. Parameters are always encoded as\\nstrings, but this field lets them be interpreted as other primitive types.\",\n      \"type\": \"string\"\n    },\n    \"map\": {\n      \"description\": \"map is the default value of the parameter if the parameter is a map.\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"name\": {\n      \"description\": \"name is the name identifying a parameter.\",\n      \"type\": \"string\"\n    },\n    \"required\": {\n      \"description\": \"required defines if this given parameter is mandatory.\",\n      \"type\": \"boolean\"\n    },\n    \"string\": {\n      \"description\": \"string is the default value of the parameter if the parameter is a string.\",\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"\
  description\": \"title is a human-readable text of the parameter name.\",\n      \"type\": \"string\"\n    },\n    \"tooltip\": {\n      \"description\": \"tooltip is a human-readable description of the parameter.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-parameter-announcement-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: repositoryParameterAnnouncement
---
