---
description: An endpoint for ingesting source content for a Channel.
layout: schema
name: IngestEndpoint
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Password
  type: object
- description: ''
  name: Url
  type: object
- description: ''
  name: Username
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-ingest-endpoint-schema.json
slug: mediapackage-api-ingest-endpoint
source_filename: mediapackage-api-ingest-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-ingest-endpoint-schema.json\",\n  \"title\": \"IngestEndpoint\",\n  \"description\": \"An endpoint for ingesting source content for a Channel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"The system generated unique identifier for the IngestEndpoint\"\n        }\n      ]\n    },\n    \"Password\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"password\"\n          },\n          \"description\": \"The system generated password for ingest authentication.\"\
  \n        }\n      ]\n    },\n    \"Url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"url\"\n          },\n          \"description\": \"The ingest URL to which the source stream should be sent.\"\n        }\n      ]\n    },\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"username\"\n          },\n          \"description\": \"The system generated username for ingest authentication.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-ingest-endpoint-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: IngestEndpoint
---
