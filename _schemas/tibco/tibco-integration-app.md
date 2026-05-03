---
description: An integration application in TIBCO Cloud Integration, representing a Flogo, BusinessWorks, or Node.js app that defines integration flows, connections, and deployment configuration.
layout: schema
name: TIBCO Cloud Integration App
properties_list:
- description: Unique identifier for the integration app
  name: id
  type: string
- description: Name of the integration app
  name: name
  type: string
- description: Description of the integration app
  name: description
  type: string
- description: Integration app type determining the runtime engine
  name: type
  type: string
- description: Current operational status of the app
  name: status
  type: string
- description: App version identifier
  name: version
  type: string
- description: When the app was created
  name: createdTime
  type: string
- description: When the app was last modified
  name: modifiedTime
  type: string
- description: User who created the app
  name: createdBy
  type: string
- description: Integration flows defined within the app
  name: flows
  type: array
- description: Connections used by the app
  name: connections
  type: array
provider_name: TIBCO
provider_slug: tibco
schema_file: json-schema/tibco-integration-app-schema.json
slug: tibco-integration-app
source_filename: tibco-integration-app-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.tibco.com/schemas/tibco/integration-app.json\",\n  \"title\": \"TIBCO Cloud Integration App\",\n  \"description\": \"An integration application in TIBCO Cloud Integration, representing a Flogo, BusinessWorks, or Node.js app that defines integration flows, connections, and deployment configuration.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"type\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the integration app\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the integration app\",\n      \"minLength\": 1,\n      \"maxLength\": 256\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the integration app\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"flogo\", \"businessworks\"\
  , \"node\"],\n      \"description\": \"Integration app type determining the runtime engine\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"draft\", \"running\", \"stopped\", \"error\"],\n      \"description\": \"Current operational status of the app\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"App version identifier\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the app was created\"\n    },\n    \"modifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the app was last modified\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"User who created the app\"\n    },\n    \"flows\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Flow\"\n      },\n      \"description\": \"Integration flows defined within the app\"\n    },\n\
  \    \"connections\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ConnectionRef\"\n      },\n      \"description\": \"Connections used by the app\"\n    }\n  },\n  \"$defs\": {\n    \"Flow\": {\n      \"type\": \"object\",\n      \"description\": \"An integration flow defining a sequence of activities triggered by an event\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Flow unique identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Flow name\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Flow description\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Flow trigger type (e.g., REST, Timer, Message)\"\n        }\n      }\n    },\n    \"ConnectionRef\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a connector\
  \ connection used by the app\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Connection identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Connection name\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Connector type\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tibco/refs/heads/main/json-schema/tibco-integration-app-schema.json
tags:
- Analytics
- API Management
- Cloud
- Enterprise Software
- Integration
- Messaging
- Real-Time Data
title: TIBCO Cloud Integration App
---
