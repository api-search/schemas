---
description: Represents a CDN-enabled backend service resource, including its CDN caching policy, backends, health checks, and protocol configuration.
layout: schema
name: Google Cloud CDN Backend Service
properties_list:
- description: The unique identifier for the resource.
  name: id
  type: string
- description: Name of the resource.
  name: name
  type: string
- description: An optional description of this resource.
  name: description
  type: string
- description: Server-defined URL for the resource.
  name: selfLink
  type: string
- description: The protocol this backend service uses to communicate with backends.
  name: protocol
  type: string
- description: If true, enables Cloud CDN for the backend service.
  name: enableCDN
  type: boolean
- description: Cloud CDN configuration for this backend service.
  name: cdnPolicy
  type: object
- description: The list of backends that serve this backend service.
  name: backends
  type: array
- description: The list of URLs to the health check resources.
  name: healthChecks
  type: array
- description: Creation timestamp in RFC3339 text format.
  name: creationTimestamp
  type: string
provider_name: Google Cloud CDN
provider_slug: google-cloud-cdn
schema_file: json-schema/cdn-backendservice.json
slug: cdn-backendservice
source_filename: cdn-backendservice.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-search/google-cloud-cdn/refs/heads/main/json-schema/cdn-backendservice.json\",\n  \"title\": \"Google Cloud CDN Backend Service\",\n  \"description\": \"Represents a CDN-enabled backend service resource, including its CDN caching policy, backends, health checks, and protocol configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the resource.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the resource.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"An optional description of this resource.\"\n    },\n    \"selfLink\": {\n      \"type\": \"string\",\n      \"description\": \"Server-defined URL for the resource.\"\n    },\n    \"protocol\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"The protocol this backend service uses to communicate with backends.\",\n      \"enum\": [\n        \"HTTP\",\n        \"HTTPS\",\n        \"HTTP2\",\n        \"TCP\",\n        \"SSL\"\n      ]\n    },\n    \"enableCDN\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, enables Cloud CDN for the backend service.\"\n    },\n    \"cdnPolicy\": {\n      \"type\": \"object\",\n      \"description\": \"Cloud CDN configuration for this backend service.\",\n      \"properties\": {\n        \"cacheMode\": {\n          \"type\": \"string\",\n          \"description\": \"Specifies the cache setting for all responses from this backend.\",\n          \"enum\": [\n            \"USE_ORIGIN_HEADERS\",\n            \"FORCE_CACHE_ALL\",\n            \"CACHE_ALL_STATIC\"\n          ]\n        },\n        \"defaultTtl\": {\n          \"type\": \"integer\",\n          \"description\": \"Default TTL for cached content in seconds.\"\n        },\n        \"maxTtl\"\
  : {\n          \"type\": \"integer\",\n          \"description\": \"Maximum allowed TTL for cached content in seconds.\"\n        },\n        \"clientTtl\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum TTL allowed in the Cache-Control response directive.\"\n        },\n        \"negativeCaching\": {\n          \"type\": \"boolean\",\n          \"description\": \"Negative caching allows caching of certain non-successful responses.\"\n        },\n        \"signedUrlCacheMaxAgeSec\": {\n          \"type\": \"string\",\n          \"description\": \"Maximum number of seconds the response to a signed URL request will be cached.\"\n        }\n      }\n    },\n    \"backends\": {\n      \"type\": \"array\",\n      \"description\": \"The list of backends that serve this backend service.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"group\": {\n            \"type\": \"string\"\n          },\n          \"balancingMode\"\
  : {\n            \"type\": \"string\"\n          },\n          \"capacityScaler\": {\n            \"type\": \"number\"\n          }\n        }\n      }\n    },\n    \"healthChecks\": {\n      \"type\": \"array\",\n      \"description\": \"The list of URLs to the health check resources.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"creationTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp in RFC3339 text format.\"\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-cdn/refs/heads/main/json-schema/cdn-backendservice.json
tags:
- Caching
- CDN
- Content Delivery
- Google Cloud
- Networking
title: Google Cloud CDN Backend Service
---
