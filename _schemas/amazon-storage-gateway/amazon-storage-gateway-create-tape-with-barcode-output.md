---
description: CreateTapeOutput
layout: schema
name: CreateTapeWithBarcodeOutput
properties_list:
- description: ''
  name: TapeARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-create-tape-with-barcode-output-schema.json
slug: amazon-storage-gateway-create-tape-with-barcode-output
source_filename: amazon-storage-gateway-create-tape-with-barcode-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-tape-with-barcode-output-schema.json\",\n  \"title\": \"CreateTapeWithBarcodeOutput\",\n  \"description\": \"CreateTapeOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TapeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeARN\"\n        },\n        {\n          \"description\": \"A unique Amazon Resource Name (ARN) that represents the virtual tape that was created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-tape-with-barcode-output-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: CreateTapeWithBarcodeOutput
---
