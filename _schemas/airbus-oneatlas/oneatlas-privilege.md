---
description: ''
layout: schema
name: Privilege
properties_list:
- description: The creation time of the created Privilege. This is returned when the Privilege is properly created.
  name: createdAt
  type: string
- description: Filters the scope of the privilege (e.g. by workspace, id)
  name: filter
  type: object
- description: ''
  name: id
  type: object
- description: The priority of the privilege
  name: priority
  type: integer
- description: List of rights granted to a user. For now, only "browse" is supported. Therefore, it will give all the rights for now.
  name: rights
  type: object
- description: ''
  name: subscriptionId
  type: object
- description: ''
  name: userId
  type: object
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-privilege-schema.json
slug: oneatlas-privilege
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-privilege-schema.json\",\n  \"title\": \"Privilege\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createdAt\": {\n      \"description\": \"The creation time of the created Privilege. This is returned when the Privilege is properly created.\",\n      \"format\": \"datetime\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"filter\": {\n      \"description\": \"Filters the scope of the privilege (e.g. by workspace, id)\",\n      \"properties\": {\n        \"id\": {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        \"workspace\": {\n          \"$ref\": \"#/components/schemas/WorkspaceIdentifier\"\n        }\n      },\n      \"required\": [\n        \"workspace\"\n      ],\n      \"type\": \"object\"\n    },\n    \"id\": {\n      \"$ref\": \"#/components/schemas/Id\"\
  \n    },\n    \"priority\": {\n      \"description\": \"The priority of the privilege\",\n      \"example\": 10,\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"rights\": {\n      \"description\": \"List of rights granted to a user. For now, only \\\"browse\\\" is supported. Therefore, it will give all the rights for now.\",\n      \"properties\": {\n        \"browse\": {\n          \"description\": \"Indicates that the user is granted the right to browse the target of the privilege\",\n          \"type\": \"object\"\n        },\n        \"buffer\": {\n          \"description\": \"Indicates that the user is granted the right to request buffer dissemination\",\n          \"type\": \"object\"\n        },\n        \"download\": {\n          \"description\": \"Indicates that the user is granted the right to request download dissemination\",\n          \"type\": \"object\"\n        },\n        \"wms\": {\n          \"description\": \"Indicates that the user is granted\
  \ the right to request WMS disseminatione\",\n          \"type\": \"object\"\n        },\n        \"wmts\": {\n          \"description\": \"Indicates that the user is granted the right to request WMTS dissemination\",\n          \"type\": \"object\"\n        }\n      },\n      \"type\": \"object\"\n    },\n    \"subscriptionId\": {\n      \"$ref\": \"#/components/schemas/Id\"\n    },\n    \"userId\": {\n      \"$ref\": \"#/components/schemas/Id\"\n    }\n  },\n  \"required\": [\n    \"userId\",\n    \"filter\",\n    \"rights\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-privilege-schema.json
tags:
- Imagery
- Satellites
title: Privilege
---
