---
description: The settings for a PUSH type input.
layout: schema
name: InputDestination
properties_list:
- description: ''
  name: Ip
  type: object
- description: ''
  name: Port
  type: object
- description: ''
  name: Url
  type: object
- description: ''
  name: Vpc
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-destination-schema.json
slug: medialive-api-input-destination
source_filename: medialive-api-input-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-destination-schema.json\",\n  \"title\": \"InputDestination\",\n  \"description\": \"The settings for a PUSH type input.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Ip\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ip\"\n          },\n          \"description\": \"The system-generated static IP address of endpoint.\\nIt remains fixed for the lifetime of the input.\\n\"\n        }\n      ]\n    },\n    \"Port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"port\"\n          },\n          \"description\": \"The port number for the input.\"\n        }\n\
  \      ]\n    },\n    \"Url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"url\"\n          },\n          \"description\": \"This represents the endpoint that the customer stream will be\\npushed to.\\n\"\n        }\n      ]\n    },\n    \"Vpc\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDestinationVpc\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vpc\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-destination-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: InputDestination
---
