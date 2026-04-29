---
description: ConfigureLogsResponse schema from Amazon MediaPackage API
layout: schema
name: ConfigureLogsResponse
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: EgressAccessLogs
  type: object
- description: ''
  name: HlsIngest
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: IngressAccessLogs
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-configure-logs-response-schema.json
slug: mediapackage-api-configure-logs-response
source_filename: mediapackage-api-configure-logs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-configure-logs-response-schema.json\",\n  \"title\": \"ConfigureLogsResponse\",\n  \"description\": \"ConfigureLogsResponse schema from Amazon MediaPackage API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) assigned to the Channel.\"\n        }\n      ]\n    },\n    \"CreatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"createdAt\"\n          },\n          \"description\": \"The date and time the Channel was created.\"\
  \n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"A short text description of the Channel.\"\n        }\n      ]\n    },\n    \"EgressAccessLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EgressAccessLogs\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"egressAccessLogs\"\n          }\n        }\n      ]\n    },\n    \"HlsIngest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsIngest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hlsIngest\"\n          }\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n\
  \          },\n          \"description\": \"The ID of the Channel.\"\n        }\n      ]\n    },\n    \"IngressAccessLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IngressAccessLogs\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ingressAccessLogs\"\n          }\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-configure-logs-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ConfigureLogsResponse
---
