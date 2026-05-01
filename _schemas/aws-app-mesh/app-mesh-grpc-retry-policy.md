---
description: An object that represents a retry policy. Specify at least one value for at least one of the types of <code>RetryEvents</code>, a value for <code>maxRetries</code>, and a value for <code>perRetryTimeout</code>. Both <code>server-error</code> and <code>gateway-error</code> under <code>httpRetryEvents</code> include the Envoy <code>reset</code> policy. For more information on the <code>reset</code> policy, see the <a href="https://www.envoyproxy.io/docs/envoy/latest/configuration/http/http_filters/router_filter#x-envoy-retry-on">Envoy documentation</a>.
layout: schema
name: GrpcRetryPolicy
properties_list:
- description: ''
  name: grpcRetryEvents
  type: object
- description: ''
  name: httpRetryEvents
  type: object
- description: ''
  name: maxRetries
  type: object
- description: ''
  name: perRetryTimeout
  type: object
- description: ''
  name: tcpRetryEvents
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-grpc-retry-policy-schema.json
slug: app-mesh-grpc-retry-policy
source_filename: app-mesh-grpc-retry-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"grpcRetryEvents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GrpcRetryPolicyEvents\"\n        },\n        {\n          \"description\": \"Specify at least one of the valid values.\"\n        }\n      ]\n    },\n    \"httpRetryEvents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpRetryPolicyEvents\"\n        },\n        {\n          \"description\": \"<p>Specify at least one of the following values.</p> <ul> <li> <p> <b>server-error</b> \\u2013 HTTP status codes 500, 501, 502, 503, 504, 505, 506, 507, 508, 510, and 511</p> </li> <li> <p> <b>gateway-error</b> \\u2013 HTTP status codes 502, 503, and 504</p> </li> <li> <p> <b>client-error</b> \\u2013 HTTP status code 409</p> </li> <li> <p> <b>stream-error</b> \\u2013 Retry on refused stream</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"maxRetries\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/MaxRetries\"\n        },\n        {\n          \"description\": \"The maximum number of retry attempts.\"\n        }\n      ]\n    },\n    \"perRetryTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Duration\"\n        },\n        {\n          \"description\": \"The timeout for each retry attempt.\"\n        }\n      ]\n    },\n    \"tcpRetryEvents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TcpRetryPolicyEvents\"\n        },\n        {\n          \"description\": \"Specify a valid value. The event occurs before any processing of a request has started and is encountered when the upstream is temporarily or permanently unavailable.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"maxRetries\",\n    \"perRetryTimeout\"\n  ],\n  \"description\": \"An object that represents a retry policy. Specify at least one value for at least one of the types of <code>RetryEvents</code>, a\
  \ value for <code>maxRetries</code>, and a value for <code>perRetryTimeout</code>. Both <code>server-error</code> and <code>gateway-error</code> under <code>httpRetryEvents</code> include the Envoy <code>reset</code> policy. For more information on the <code>reset</code> policy, see the <a href=\\\"https://www.envoyproxy.io/docs/envoy/latest/configuration/http/http_filters/router_filter#x-envoy-retry-on\\\">Envoy documentation</a>.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-retry-policy-schema.json\",\n  \"title\": \"GrpcRetryPolicy\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-grpc-retry-policy-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: GrpcRetryPolicy
---
