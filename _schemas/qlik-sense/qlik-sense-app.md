---
description: Schema representing a Qlik Sense analytics application in Qlik Cloud, including its metadata, ownership, space assignment, and reload information.
layout: schema
name: Qlik Sense App
properties_list:
- description: The unique identifier of the app, assigned by the Qlik Cloud platform.
  name: id
  type: string
- description: The display name of the app.
  name: name
  type: string
- description: A human-readable description of the app and its purpose.
  name: description
  type: string
- description: URL to the app thumbnail image.
  name: thumbnail
  type: string
- description: The date and time of the most recent successful data reload in ISO 8601 format.
  name: lastReloadTime
  type: string
- description: The date and time when the app was initially created.
  name: createdDate
  type: string
- description: The date and time when the app was last modified.
  name: modifiedDate
  type: string
- description: The display name of the app owner.
  name: owner
  type: string
- description: The unique identifier of the user who owns the app.
  name: ownerId
  type: string
- description: Indicates whether the app has been published to a managed space.
  name: published
  type: boolean
- description: The date and time when the app was published. Null if the app is not published.
  name: publishTime
  type: string
- description: Custom properties assigned to the app as key-value pairs.
  name: custom
  type: object
- description: A color expression evaluated dynamically for the app representation in the hub.
  name: dynamicColor
  type: string
- description: Indicates whether the app uses section access for row-level security.
  name: hasSectionAccess
  type: boolean
- description: Indicates whether the app operates in Direct Query mode, querying data sources in real time rather than loading data into memory.
  name: isDirectQueryMode
  type: boolean
- description: Indicates whether the app data is encrypted at rest using customer-managed keys.
  name: encrypted
  type: boolean
- description: The identifier of the origin app if this app was created by copying or publishing another app.
  name: originAppId
  type: string
- description: The identifier of the space containing the app. Null if the app is in the personal space.
  name: spaceId
  type: string
- description: The identifier of the Qlik Cloud tenant the app belongs to.
  name: tenantId
  type: string
- description: The intended use case for the app.
  name: usage
  type: string
- description: HATEOAS links for navigating related resources.
  name: links
  type: object
- description: Reference to the space containing this app.
  name: space
  type: object
- description: Reference to the most recent reload of this app.
  name: reload
  type: object
provider_name: Qlik Sense
provider_slug: qlik-sense
schema_file: json-schema/qlik-sense-app-schema.json
slug: qlik-sense-app
source_filename: qlik-sense-app-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://qlik.dev/schemas/qlik-sense-app-schema.json\",\n  \"title\": \"Qlik Sense App\",\n  \"description\": \"Schema representing a Qlik Sense analytics application in Qlik Cloud, including its metadata, ownership, space assignment, and reload information.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"name\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the app, assigned by the Qlik Cloud platform.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the app.\",\n      \"maxLength\": 256\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the app and its purpose.\"\n    },\n    \"thumbnail\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to\
  \ the app thumbnail image.\"\n    },\n    \"lastReloadTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time of the most recent successful data reload in ISO 8601 format.\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the app was initially created.\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the app was last modified.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the app owner.\"\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the user who owns the app.\"\n    },\n    \"published\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the app has been published to a managed space.\",\n   \
  \   \"default\": false\n    },\n    \"publishTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the app was published. Null if the app is not published.\"\n    },\n    \"custom\": {\n      \"type\": \"object\",\n      \"description\": \"Custom properties assigned to the app as key-value pairs.\",\n      \"additionalProperties\": true\n    },\n    \"dynamicColor\": {\n      \"type\": \"string\",\n      \"description\": \"A color expression evaluated dynamically for the app representation in the hub.\"\n    },\n    \"hasSectionAccess\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the app uses section access for row-level security.\",\n      \"default\": false\n    },\n    \"isDirectQueryMode\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the app operates in Direct Query mode, querying data sources in real time rather than loading data into memory.\",\n  \
  \    \"default\": false\n    },\n    \"encrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the app data is encrypted at rest using customer-managed keys.\",\n      \"default\": false\n    },\n    \"originAppId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the origin app if this app was created by copying or publishing another app.\"\n    },\n    \"spaceId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the space containing the app. Null if the app is in the personal space.\"\n    },\n    \"tenantId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the Qlik Cloud tenant the app belongs to.\"\n    },\n    \"usage\": {\n      \"type\": \"string\",\n      \"description\": \"The intended use case for the app.\",\n      \"enum\": [\n        \"ANALYTICS\",\n        \"DATA_PREPARATION\",\n        \"DATAFLOW_PREP\"\n      ]\n    },\n    \"links\": {\n      \"type\": \"\
  object\",\n      \"description\": \"HATEOAS links for navigating related resources.\",\n      \"properties\": {\n        \"self\": {\n          \"$ref\": \"#/$defs/Link\"\n        },\n        \"open\": {\n          \"$ref\": \"#/$defs/Link\"\n        },\n        \"thumbnail\": {\n          \"$ref\": \"#/$defs/Link\"\n        }\n      }\n    },\n    \"space\": {\n      \"$ref\": \"#/$defs/SpaceReference\",\n      \"description\": \"Reference to the space containing this app.\"\n    },\n    \"reload\": {\n      \"$ref\": \"#/$defs/ReloadReference\",\n      \"description\": \"Reference to the most recent reload of this app.\"\n    }\n  },\n  \"$defs\": {\n    \"Link\": {\n      \"type\": \"object\",\n      \"description\": \"A hypermedia link.\",\n      \"properties\": {\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL of the linked resource.\"\n        }\n      },\n      \"required\": [\n        \"href\"\n      ]\n\
  \    },\n    \"SpaceReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a Qlik Cloud space that contains and governs access to resources.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the space.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the space.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of space.\",\n          \"enum\": [\n            \"shared\",\n            \"managed\",\n            \"data\"\n          ]\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A human-readable description of the space.\"\n        },\n        \"ownerId\": {\n          \"type\": \"string\",\n          \"description\": \"The identifier of the space owner.\"\n        },\n        \"tenantId\": {\n  \
  \        \"type\": \"string\",\n          \"description\": \"The identifier of the tenant the space belongs to.\"\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the space was created.\"\n        },\n        \"updatedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the space was last updated.\"\n        }\n      },\n      \"required\": [\n        \"id\",\n        \"name\",\n        \"type\"\n      ]\n    },\n    \"ReloadReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a data reload operation for a Qlik Sense app.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the reload.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The current status of the reload.\",\n\
  \          \"enum\": [\n            \"QUEUED\",\n            \"RELOADING\",\n            \"CANCELING\",\n            \"SUCCEEDED\",\n            \"FAILED\",\n            \"CANCELED\",\n            \"EXCEEDED_LIMIT\"\n          ]\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"How the reload was triggered.\",\n          \"enum\": [\n            \"hub\",\n            \"external\",\n            \"chronos\",\n            \"automations\"\n          ]\n        },\n        \"partial\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this was a partial reload.\",\n          \"default\": false\n        },\n        \"creationTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the reload was created.\"\n        },\n        \"startTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the reload started\
  \ executing.\"\n        },\n        \"endTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the reload finished.\"\n        },\n        \"duration\": {\n          \"type\": \"string\",\n          \"description\": \"The duration of the reload in ISO 8601 duration format.\"\n        }\n      },\n      \"required\": [\n        \"id\",\n        \"status\"\n      ]\n    },\n    \"SpaceAssignment\": {\n      \"type\": \"object\",\n      \"description\": \"A role assignment for a user or group within a space.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the assignment.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Whether the assignee is a user or group.\",\n          \"enum\": [\n            \"user\",\n            \"group\"\n          ]\n        },\n        \"assigneeId\": {\n          \"\
  type\": \"string\",\n          \"description\": \"The identifier of the assigned user or group.\"\n        },\n        \"roles\": {\n          \"type\": \"array\",\n          \"description\": \"The roles granted to the assignee in this space.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"consumer\",\n              \"contributor\",\n              \"dataconsumer\",\n              \"facilitator\",\n              \"manager\",\n              \"operator\",\n              \"producer\",\n              \"publisher\",\n              \"basicconsumer\"\n            ]\n          }\n        },\n        \"spaceId\": {\n          \"type\": \"string\",\n          \"description\": \"The space this assignment applies to.\"\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the assignment was created.\"\n        },\n        \"updatedAt\": {\n          \"type\"\
  : \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the assignment was last updated.\"\n        }\n      },\n      \"required\": [\n        \"id\",\n        \"type\",\n        \"assigneeId\",\n        \"roles\"\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/qlik-sense/refs/heads/main/json-schema/qlik-sense-app-schema.json
tags:
- Analytics
- Business Intelligence
- Cloud
- Data Integration
- Visualization
title: Qlik Sense App
---
