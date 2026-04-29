---
description: A Worker script object from the Cloudflare API, representing serverless code deployed to Cloudflare's global edge network with associated configuration, bindings, and deployment metadata.
layout: schema
name: Cloudflare Worker Script
properties_list:
- description: The unique identifier of the Worker script, typically the script name.
  name: id
  type: string
- description: A unique tag for the Worker script used for caching and versioning.
  name: tag
  type: string
- description: The entity tag for cache validation.
  name: etag
  type: string
- description: List of event handlers the Worker implements (e.g., fetch, scheduled, queue).
  name: handlers
  type: array
- description: Named handlers for Durable Objects and other named event handling.
  name: named_handlers
  type: array
- description: The compatibility date for the Worker runtime.
  name: compatibility_date
  type: string
- description: Compatibility flags enabled for the Worker.
  name: compatibility_flags
  type: array
- description: The usage model for billing.
  name: usage_model
  type: string
- description: Environment bindings configured for the Worker.
  name: bindings
  type: array
- description: Routes that trigger this Worker.
  name: routes
  type: array
- description: Whether Logpush is enabled for the Worker.
  name: logpush
  type: boolean
- description: Smart placement configuration.
  name: placement
  type: object
- description: Workers that receive tail events from this Worker.
  name: tail_consumers
  type: array
- description: When the Worker script was created.
  name: created_on
  type: string
- description: When the Worker script was last modified.
  name: modified_on
  type: string
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-worker-script-schema.json
slug: cloudflare-worker-script
source_filename: cloudflare-worker-script-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-worker-script-schema.json\",\n  \"title\": \"Cloudflare Worker Script\",\n  \"description\": \"A Worker script object from the Cloudflare API, representing serverless code deployed to Cloudflare's global edge network with associated configuration, bindings, and deployment metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"id\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the Worker script, typically the script name.\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"description\": \"A unique tag for the Worker script used for caching and versioning.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The entity tag for cache validation.\"\n    },\n    \"handlers\": {\n      \"\
  type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of event handlers the Worker implements (e.g., fetch, scheduled, queue).\"\n    },\n    \"named_handlers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The handler name.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The handler type.\"\n          }\n        }\n      },\n      \"description\": \"Named handlers for Durable Objects and other named event handling.\"\n    },\n    \"compatibility_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The compatibility date for the Worker runtime.\"\n    },\n    \"compatibility_flags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\"\
  : \"Compatibility flags enabled for the Worker.\"\n    },\n    \"usage_model\": {\n      \"type\": \"string\",\n      \"description\": \"The usage model for billing.\",\n      \"enum\": [\"bundled\", \"unbound\", \"standard\"]\n    },\n    \"bindings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Binding\"\n      },\n      \"description\": \"Environment bindings configured for the Worker.\"\n    },\n    \"routes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Route identifier.\"\n          },\n          \"pattern\": {\n            \"type\": \"string\",\n            \"description\": \"URL pattern for the route.\"\n          },\n          \"zone_name\": {\n            \"type\": \"string\",\n            \"description\": \"Zone name for the route.\"\n          }\n        }\n      },\n      \"description\":\
  \ \"Routes that trigger this Worker.\"\n    },\n    \"logpush\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Logpush is enabled for the Worker.\"\n    },\n    \"placement\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"mode\": {\n          \"type\": \"string\",\n          \"description\": \"The placement mode for the Worker.\",\n          \"enum\": [\"smart\"]\n        }\n      },\n      \"description\": \"Smart placement configuration.\"\n    },\n    \"tail_consumers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"service\": {\n            \"type\": \"string\",\n            \"description\": \"The tail consumer Worker service name.\"\n          }\n        }\n      },\n      \"description\": \"Workers that receive tail events from this Worker.\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When\
  \ the Worker script was created.\"\n    },\n    \"modified_on\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the Worker script was last modified.\"\n    }\n  },\n  \"$defs\": {\n    \"Binding\": {\n      \"type\": \"object\",\n      \"required\": [\"name\", \"type\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The binding variable name accessible in the Worker code.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of binding.\",\n          \"enum\": [\n            \"kv_namespace\",\n            \"durable_object_namespace\",\n            \"r2_bucket\",\n            \"d1\",\n            \"service\",\n            \"queue\",\n            \"ai\",\n            \"vectorize\",\n            \"hyperdrive\",\n            \"secret_text\",\n            \"plain_text\",\n            \"browser\",\n            \"analytics_engine\"\
  \n          ]\n        },\n        \"namespace_id\": {\n          \"type\": \"string\",\n          \"description\": \"Namespace ID for KV or Durable Object bindings.\"\n        },\n        \"bucket_name\": {\n          \"type\": \"string\",\n          \"description\": \"Bucket name for R2 bindings.\"\n        },\n        \"database_id\": {\n          \"type\": \"string\",\n          \"description\": \"Database ID for D1 bindings.\"\n        },\n        \"queue_name\": {\n          \"type\": \"string\",\n          \"description\": \"Queue name for Queue bindings.\"\n        },\n        \"service\": {\n          \"type\": \"string\",\n          \"description\": \"Service name for service bindings.\"\n        },\n        \"text\": {\n          \"type\": \"string\",\n          \"description\": \"Value for plain text bindings.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-worker-script-schema.json
tags:
- AI Gateway
- API Gateway
- Artificial Intelligence
- CDN
- Cloud
- Containers
- DDoS Protection
- DNS
- Edge
- Edge Computing
- Object Storage
- Platform
- Real-Time Communication
- Security
- Serverless
- Web Performance
title: Cloudflare Worker Script
---
