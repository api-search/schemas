---
description: Schema for a BeyondCorp app connection resource that defines a secure connection to a private application endpoint through BeyondCorp.
layout: schema
name: Google BeyondCorp App Connection
properties_list:
- description: The resource name of the app connection
  name: name
  type: string
- description: User-friendly display name for the app connection
  name: displayName
  type: string
- description: Unique identifier of the app connection
  name: uid
  type: string
- description: The type of network connectivity used by the connection
  name: type
  type: string
- description: The endpoint of the application to connect to
  name: applicationEndpoint
  type: object
- description: Resource names of app connectors associated with this connection
  name: connectors
  type: array
- description: Current state of the app connection
  name: state
  type: string
- description: Gateway information for the connection
  name: gateway
  type: object
- description: Labels applied to the app connection
  name: labels
  type: object
- description: Timestamp when the connection was created
  name: createTime
  type: string
- description: Timestamp when the connection was last updated
  name: updateTime
  type: string
provider_name: Google BeyondCorp
provider_slug: google-beyondcorp
schema_file: json-schema/google-beyondcorp-app-connection-schema.json
slug: google-beyondcorp-app-connection
source_filename: google-beyondcorp-app-connection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://cloud.google.com/schemas/beyondcorp/app-connection.json\",\n  \"title\": \"Google BeyondCorp App Connection\",\n  \"description\": \"Schema for a BeyondCorp app connection resource that defines a secure connection to a private application endpoint through BeyondCorp.\",\n  \"type\": \"object\",\n  \"required\": [\"applicationEndpoint\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the app connection\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"User-friendly display name for the app connection\"\n    },\n    \"uid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the app connection\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of network connectivity used by the connection\",\n      \"enum\": [\"TYPE_UNSPECIFIED\"\
  , \"TCP_PROXY\"]\n    },\n    \"applicationEndpoint\": {\n      \"$ref\": \"#/$defs/ApplicationEndpoint\",\n      \"description\": \"The endpoint of the application to connect to\"\n    },\n    \"connectors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Resource names of app connectors associated with this connection\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current state of the app connection\",\n      \"enum\": [\"STATE_UNSPECIFIED\", \"CREATING\", \"CREATED\", \"UPDATING\", \"DELETING\", \"DOWN\"]\n    },\n    \"gateway\": {\n      \"$ref\": \"#/$defs/Gateway\",\n      \"description\": \"Gateway information for the connection\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels applied to the app connection\"\n    },\n    \"createTime\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the connection was created\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the connection was last updated\"\n    }\n  },\n  \"$defs\": {\n    \"ApplicationEndpoint\": {\n      \"type\": \"object\",\n      \"description\": \"The endpoint of the application to connect to\",\n      \"required\": [\"host\", \"port\"],\n      \"properties\": {\n        \"host\": {\n          \"type\": \"string\",\n          \"description\": \"Hostname or IP address of the application\"\n        },\n        \"port\": {\n          \"type\": \"integer\",\n          \"description\": \"Port of the application\",\n          \"minimum\": 1,\n          \"maximum\": 65535\n        }\n      }\n    },\n    \"Gateway\": {\n      \"type\": \"object\",\n      \"description\": \"Gateway configuration for the app connection\",\n      \"properties\": {\n     \
  \   \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of gateway hosting the connection\",\n          \"enum\": [\"TYPE_UNSPECIFIED\", \"GCP_REGIONAL_MIG\"]\n        },\n        \"uri\": {\n          \"type\": \"string\",\n          \"description\": \"The URI of the gateway\"\n        },\n        \"ingressPort\": {\n          \"type\": \"integer\",\n          \"description\": \"The ingress port of the gateway\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-beyondcorp/refs/heads/main/json-schema/google-beyondcorp-app-connection-schema.json
tags:
- Access Control
- Enterprise Security
- Identity
- Security
- VPN Alternative
- Zero Trust
title: Google BeyondCorp App Connection
---
