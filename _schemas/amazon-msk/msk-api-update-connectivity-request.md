---
description: Request body for UpdateConnectivity.
layout: schema
name: UpdateConnectivityRequest
properties_list:
- description: ''
  name: ConnectivityInfo
  type: object
- description: ''
  name: CurrentVersion
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-update-connectivity-request-schema.json
slug: msk-api-update-connectivity-request
source_filename: msk-api-update-connectivity-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-connectivity-request-schema.json\",\n  \"title\": \"UpdateConnectivityRequest\",\n  \"description\": \"Request body for UpdateConnectivity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConnectivityInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectivityInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"connectivityInfo\"\n          },\n          \"description\": \"\\n            <p>Information about the broker access configuration.</p>\"\n        }\n      ]\n    },\n    \"CurrentVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"currentVersion\"\n          },\n          \"description\": \"\\n       \
  \     <p>The version of the MSK cluster to update. Cluster versions aren't simple numbers. You can describe an MSK cluster to find its version. When this update operation is successful, it generates a new cluster version.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConnectivityInfo\",\n    \"CurrentVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-connectivity-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: UpdateConnectivityRequest
---
