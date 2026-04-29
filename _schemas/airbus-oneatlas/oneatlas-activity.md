---
description: ''
layout: schema
name: Activity
properties_list:
- description: ''
  name: _links
  type: object
- description: The time when the activity was created
  name: creationDate
  type: string
- description: The time when the activity was ended (copy of the date associated to the SUCCEEDED, CANCELED or FAILED stage)
  name: endDate
  type: string
- description: ''
  name: id
  type: object
- description: Name of the last completed stage
  name: lastStageName
  type: string
- description: A free text (copy of the last stage message)
  name: message
  type: string
- description: The copy of the origin user request
  name: payload
  type: object
- description: A priority indicator between 1 and 9. 1 is the highest.
  name: priority
  type: number
- description: A progress indicator between 0 and 100
  name: progress
  type: number
- description: The time when the activity was started (date of the first stage that is not QUEUED)
  name: startDate
  type: string
- description: Status of the activity (copy of the last stage status)
  name: status
  type: string
- description: Type of activity
  name: type
  type: string
- description: ''
  name: userId
  type: object
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-activity-schema.json
slug: oneatlas-activity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-activity-schema.json\",\n  \"title\": \"Activity\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_links\": {\n      \"properties\": {\n        \"cancel\": {\n          \"allOf\": [\n            {\n              \"description\": \"See [Cancel activity](#/paths/~1api~1v1~1activities~1{correlationId}~1cancel/post)\"\n            },\n            {\n              \"$ref\": \"#/components/schemas/Link\"\n            }\n          ]\n        },\n        \"catalogItems\": {\n          \"description\": \"Resource id property (`resourceId`) is a catalog item id (`catalogItemId`). It can be used in all endpoints that need a `catalogItemId`.\\n\\nSee [Search catalog items with opensearch](#/paths/~1api~1v1~1opensearch/get). See [Format catalog item](#/paths/~1api~1v1~1items~1{catalogItemId}~1format/post).\"\
  ,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/Link\"\n          },\n          \"type\": \"array\",\n          \"uniqueItems\": true\n        },\n        \"history\": {\n          \"allOf\": [\n            {\n              \"description\": \"See [Get activity stages](#/paths/~1api~1v1~1activities~1{correlationId}~1stages/get)\"\n            },\n            {\n              \"$ref\": \"#/components/schemas/Link\"\n            }\n          ]\n        },\n        \"hold\": {\n          \"allOf\": [\n            {\n              \"description\": \"See [Hold activity](#/paths/~1api~1v1~1activities~1{correlationId}~1hold/post)\"\n            },\n            {\n              \"$ref\": \"#/components/schemas/Link\"\n            }\n          ]\n        },\n        \"nexts\": {\n          \"description\": \"Next endpoints applicable to the resource when the activity is finished.\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/Link\"\n          },\n\
  \          \"type\": \"array\",\n          \"uniqueItems\": true\n        },\n        \"rerun\": {\n          \"allOf\": [\n            {\n              \"description\": \"See [Run activity](#/paths/~1api~1v1~1activities~1{correlationId}~1rerun/post)\"\n            },\n            {\n              \"$ref\": \"#/components/schemas/Link\"\n            }\n          ]\n        }\n      },\n      \"readOnly\": true,\n      \"type\": \"object\"\n    },\n    \"creationDate\": {\n      \"description\": \"The time when the activity was created\",\n      \"format\": \"datetime\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"endDate\": {\n      \"description\": \"The time when the activity was ended (copy of the date associated to the SUCCEEDED, CANCELED or FAILED stage)\",\n      \"format\": \"datetime\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"$ref\": \"#/components/schemas/Id\"\n    },\n    \"lastStageName\": {\n      \"description\"\
  : \"Name of the last completed stage\",\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"description\": \"A free text (copy of the last stage message)\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"payload\": {\n      \"description\": \"The copy of the origin user request\",\n      \"type\": \"object\"\n    },\n    \"priority\": {\n      \"default\": 5,\n      \"description\": \"A priority indicator between 1 and 9. 1 is the highest.\",\n      \"format\": \"int\",\n      \"maximum\": 9,\n      \"minimum\": 1,\n      \"type\": \"number\"\n    },\n    \"progress\": {\n      \"default\": 0,\n      \"description\": \"A progress indicator between 0 and 100\",\n      \"format\": \"int\",\n      \"maximum\": 100,\n      \"minimum\": 0,\n      \"type\": \"number\"\n    },\n    \"startDate\": {\n      \"description\": \"The time when the activity was started (date of the first stage that is not QUEUED)\",\n      \"format\": \"datetime\",\n      \"readOnly\"\
  : true,\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"default\": \"QUEUED\",\n      \"description\": \"Status of the activity (copy of the last stage status)\",\n      \"enum\": [\n        \"QUEUED\",\n        \"RUNNING\",\n        \"ON_HOLD\",\n        \"CANCELED\",\n        \"WAITING_CANCEL\",\n        \"SUCCEEDED\",\n        \"FAILED\",\n        \"ARCHIVED\"\n      ],\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"Type of activity\",\n      \"enum\": [\n        \"ingestion\",\n        \"process\",\n        \"format\",\n        \"control\",\n        \"deliver\"\n      ],\n      \"type\": \"string\"\n    },\n    \"userId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The id of the user that is the origin of the activity (extracted from the X-Forwarded-User request header)\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-activity-schema.json
tags:
- Imagery
- Satellites
title: Activity
---
