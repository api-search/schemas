---
description: A RequestAuthentication defines what request authentication methods are supported by a workload. It validates JSON Web Tokens (JWTs) attached to requests and extracts identity information for use in authorization policies.
layout: schema
name: Istio RequestAuthentication
properties_list:
- description: Workload selector to apply the policy to specific workloads.
  name: selector
  type: object
- description: Target references to apply the policy to specific resources.
  name: targetRefs
  type: array
- description: List of JWT rules defining the valid identity tokens for this workload.
  name: jwtRules
  type: array
provider_name: Istio
provider_slug: istio
schema_file: json-schema/request-authentication.json
slug: request-authentication
source_filename: request-authentication.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/istio/blob/main/json-schema/request-authentication.json\",\n  \"title\": \"Istio RequestAuthentication\",\n  \"description\": \"A RequestAuthentication defines what request authentication methods are supported by a workload. It validates JSON Web Tokens (JWTs) attached to requests and extracts identity information for use in authorization policies.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"selector\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"matchLabels\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"One or more labels that indicate a specific set of pods/VMs on which the policy should be applied.\"\n        }\n      },\n      \"description\": \"Workload selector to apply the policy to specific workloads.\"\n    },\n\
  \    \"targetRefs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"group\": {\n            \"type\": \"string\",\n            \"description\": \"Group of the target resource.\"\n          },\n          \"kind\": {\n            \"type\": \"string\",\n            \"description\": \"Kind of the target resource.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Name of the target resource.\"\n          }\n        }\n      },\n      \"description\": \"Target references to apply the policy to specific resources.\"\n    },\n    \"jwtRules\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"issuer\": {\n            \"type\": \"string\",\n            \"description\": \"Identifies the issuer that issued the JWT. Must match the iss claim in the JWT.\"\n          },\n          \"audiences\": {\n  \
  \          \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"The list of JWT audiences that are allowed to access. If not specified, the audiences in the JWT will not be checked.\"\n          },\n          \"jwksUri\": {\n            \"type\": \"string\",\n            \"description\": \"URL of the provider's public key set to validate the signature of the JWT.\"\n          },\n          \"jwks\": {\n            \"type\": \"string\",\n            \"description\": \"JSON Web Key Set of public keys to validate the signature of the JWT. Mutually exclusive with jwksUri.\"\n          },\n          \"fromHeaders\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\",\n                  \"description\": \"The HTTP header name.\"\n                },\n                \"\
  prefix\": {\n                  \"type\": \"string\",\n                  \"description\": \"The prefix that should be stripped before decoding the token.\"\n                }\n              },\n              \"required\": [\"name\"]\n            },\n            \"description\": \"List of header locations from which JWT is expected.\"\n          },\n          \"fromParams\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"List of query parameters from which JWT is expected.\"\n          },\n          \"fromCookies\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"List of cookie names from which JWT is expected.\"\n          },\n          \"outputPayloadToHeader\": {\n            \"type\": \"string\",\n            \"description\": \"This field specifies the header name to output a successfully verified\
  \ JWT payload to the backend.\"\n          },\n          \"forwardOriginalToken\": {\n            \"type\": \"boolean\",\n            \"description\": \"If set to true, the original JWT will be preserved in the Authorization header for upstream service.\"\n          },\n          \"outputClaimToHeaders\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"header\": {\n                  \"type\": \"string\",\n                  \"description\": \"The name of the header to be created.\"\n                },\n                \"claim\": {\n                  \"type\": \"string\",\n                  \"description\": \"The name of the claim to be copied from.\"\n                }\n              }\n            },\n            \"description\": \"List of claim-to-header mappings to extract JWT claims and output them to request headers.\"\n          },\n          \"timeout\": {\n            \"type\"\
  : \"string\",\n            \"description\": \"Timeout for JWKS fetch operations.\"\n          }\n        },\n        \"required\": [\"issuer\"]\n      },\n      \"description\": \"List of JWT rules defining the valid identity tokens for this workload.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/json-schema/request-authentication.json
tags:
- CNCF
- Kubernetes
- Microservices
- Open Source
- Service Mesh
title: Istio RequestAuthentication
---
