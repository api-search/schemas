---
description: DirectResponse configures a Gateway to directly respond to incoming requests with a custom HTTP response code and body.
layout: schema
name: kgateway DirectResponse
properties_list:
- description: API version for the DirectResponse resource.
  name: apiVersion
  type: string
- description: Resource kind.
  name: kind
  type: string
- description: Standard Kubernetes object metadata.
  name: metadata
  type: object
- description: DirectResponseSpec defines the desired state of a DirectResponse.
  name: spec
  type: object
provider_name: Kgateway
provider_slug: kgateway
schema_file: json-schema/direct-response.json
slug: direct-response
source_filename: direct-response.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kgateway/blob/main/json-schema/direct-response.json\",\n  \"title\": \"kgateway DirectResponse\",\n  \"description\": \"DirectResponse configures a Gateway to directly respond to incoming requests with a custom HTTP response code and body.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"const\": \"gateway.kgateway.dev/v1alpha1\",\n      \"description\": \"API version for the DirectResponse resource.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"const\": \"DirectResponse\",\n      \"description\": \"Resource kind.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Standard Kubernetes object metadata.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the DirectResponse resource.\"\
  \n        },\n        \"namespace\": {\n          \"type\": \"string\",\n          \"description\": \"Namespace of the DirectResponse resource.\"\n        },\n        \"labels\": {\n          \"type\": \"object\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        },\n        \"annotations\": {\n          \"type\": \"object\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        }\n      },\n      \"required\": [\"name\"]\n    },\n    \"spec\": {\n      \"type\": \"object\",\n      \"description\": \"DirectResponseSpec defines the desired state of a DirectResponse.\",\n      \"properties\": {\n        \"statusCode\": {\n          \"type\": \"integer\",\n          \"description\": \"HTTP status code to return.\",\n          \"minimum\": 200,\n          \"maximum\": 599\n        },\n        \"body\": {\n          \"type\": \"string\",\n          \"description\": \"Response body to return.\"\n        }\n      },\n      \"required\": [\"statusCode\"]\n\
  \    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kgateway/refs/heads/main/json-schema/direct-response.json
tags:
- Gateways
title: kgateway DirectResponse
---
