---
description: Represents the metadata response from the Dapr sidecar, including application connection details, registered components, active subscriptions, HTTP endpoints, and custom extended attributes.
layout: schema
name: Dapr Metadata
properties_list:
- description: The application ID.
  name: id
  type: string
- description: The Dapr runtime version.
  name: runtimeVersion
  type: string
- description: List of enabled Dapr features.
  name: enabledFeatures
  type: array
- description: Registered actor types and their active instance counts.
  name: actors
  type: array
- description: Registered Dapr components.
  name: components
  type: array
- description: Active pub/sub subscriptions.
  name: subscriptions
  type: array
- description: Registered HTTP endpoints.
  name: httpEndpoints
  type: array
- description: Application connection properties.
  name: appConnectionProperties
  type: object
- description: Custom extended metadata attributes.
  name: extended
  type: object
provider_name: Dapr
provider_slug: dapr
schema_file: json-schema/metadata.json
slug: metadata
source_filename: metadata.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/dapr/blob/main/json-schema/metadata.json\",\n  \"title\": \"Dapr Metadata\",\n  \"description\": \"Represents the metadata response from the Dapr sidecar, including application connection details, registered components, active subscriptions, HTTP endpoints, and custom extended attributes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The application ID.\"\n    },\n    \"runtimeVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The Dapr runtime version.\"\n    },\n    \"enabledFeatures\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of enabled Dapr features.\"\n    },\n    \"actors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n     \
  \     \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The registered actor type name.\"\n          },\n          \"count\": {\n            \"type\": \"integer\",\n            \"description\": \"The number of active instances of this actor type.\"\n          }\n        }\n      },\n      \"description\": \"Registered actor types and their active instance counts.\"\n    },\n    \"components\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The component name.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The component type (e.g., state.redis, pubsub.kafka).\"\n          },\n          \"version\": {\n            \"type\": \"string\",\n            \"description\": \"The component version.\"\n          },\n          \"capabilities\": {\n            \"type\"\
  : \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"Capabilities supported by this component.\"\n          }\n        }\n      },\n      \"description\": \"Registered Dapr components.\"\n    },\n    \"subscriptions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"pubsubname\": {\n            \"type\": \"string\",\n            \"description\": \"The pub/sub component name.\"\n          },\n          \"topic\": {\n            \"type\": \"string\",\n            \"description\": \"The subscribed topic.\"\n          },\n          \"rules\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\"\n            },\n            \"description\": \"Subscription routing rules.\"\n          },\n          \"deadLetterTopic\": {\n            \"type\": \"string\",\n            \"description\": \"The dead letter topic\
  \ for failed messages.\"\n          }\n        }\n      },\n      \"description\": \"Active pub/sub subscriptions.\"\n    },\n    \"httpEndpoints\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The HTTP endpoint name.\"\n          }\n        }\n      },\n      \"description\": \"Registered HTTP endpoints.\"\n    },\n    \"appConnectionProperties\": {\n      \"type\": \"object\",\n      \"description\": \"Application connection properties.\",\n      \"properties\": {\n        \"port\": {\n          \"type\": \"integer\",\n          \"description\": \"The application port.\"\n        },\n        \"protocol\": {\n          \"type\": \"string\",\n          \"description\": \"The application protocol (http or grpc).\"\n        },\n        \"channelAddress\": {\n          \"type\": \"string\",\n          \"description\": \"The application channel\
  \ address.\"\n        },\n        \"maxConcurrency\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum concurrency level for the application.\"\n        },\n        \"health\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"healthCheckPath\": {\n              \"type\": \"string\",\n              \"description\": \"The health check endpoint path.\"\n            },\n            \"healthProbeInterval\": {\n              \"type\": \"string\",\n              \"description\": \"Interval between health probes.\"\n            },\n            \"healthProbeTimeout\": {\n              \"type\": \"string\",\n              \"description\": \"Timeout for health probes.\"\n            },\n            \"healthThreshold\": {\n              \"type\": \"integer\",\n              \"description\": \"Number of consecutive failures before unhealthy.\"\n            }\n          },\n          \"description\": \"Application health check configuration.\"\n\
  \        }\n      }\n    },\n    \"extended\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Custom extended metadata attributes.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/json-schema/metadata.json
tags:
- Distributed Systems
- Microservices
- Platform
- Pub/Sub
- State Management
- Workflows
title: Dapr Metadata
---
