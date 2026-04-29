---
description: DescribeTapesOutput
layout: schema
name: DescribeTapesOutput
properties_list:
- description: ''
  name: Tapes
  type: object
- description: ''
  name: Marker
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-tapes-output-schema.json
slug: amazon-storage-gateway-describe-tapes-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-tapes-output-schema.json\",\n  \"title\": \"DescribeTapesOutput\",\n  \"description\": \"DescribeTapesOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tapes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tapes\"\n        },\n        {\n          \"description\": \"An array of virtual tape descriptions.\"\n        }\n      ]\n    },\n    \"Marker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"<p>An opaque string that can be used as part of a subsequent <code>DescribeTapes</code> call to retrieve the next page of results.</p> <p>If a response does not contain a marker, then there are no more results to be retrieved.</p>\"\n  \
  \      }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-tapes-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeTapesOutput
---
