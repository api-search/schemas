---
description: Product information returned from a barcode lookup API query.
layout: schema
name: BarcodeLookupResponse
properties_list:
- description: The barcode number queried.
  name: barcode_number
  type: string
- description: The barcode format/symbology.
  name: barcode_type
  type: string
- description: URL of the barcode image.
  name: barcode_image
  type: string
- description: ''
  name: product
  type: object
provider_name: Barcode Scanners
provider_slug: barcode-scanners
schema_file: json-schema/barcode-lookup-schema.json
slug: barcode-lookup
source_filename: barcode-lookup-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/barcode-scanners/json-schema/barcode-lookup-schema.json\",\n  \"title\": \"BarcodeLookupResponse\",\n  \"description\": \"Product information returned from a barcode lookup API query.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"barcode_number\": {\n      \"type\": \"string\",\n      \"description\": \"The barcode number queried.\"\n    },\n    \"barcode_type\": {\n      \"type\": \"string\",\n      \"enum\": [\"UPC-A\", \"UPC-E\", \"EAN-13\", \"EAN-8\", \"ISBN-10\", \"ISBN-13\", \"QR Code\", \"Code 128\", \"Code 39\", \"Data Matrix\", \"PDF417\"],\n      \"description\": \"The barcode format/symbology.\"\n    },\n    \"barcode_image\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the barcode image.\"\n    },\n    \"product\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"title\": {\n   \
  \       \"type\": \"string\",\n          \"description\": \"Product name or title.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Product description.\"\n        },\n        \"category\": {\n          \"type\": \"string\",\n          \"description\": \"Product category.\"\n        },\n        \"brand\": {\n          \"type\": \"string\",\n          \"description\": \"Product brand or manufacturer.\"\n        },\n        \"manufacturer\": {\n          \"type\": \"string\",\n          \"description\": \"Product manufacturer name.\"\n        },\n        \"mpn\": {\n          \"type\": \"string\",\n          \"description\": \"Manufacturer Part Number.\"\n        },\n        \"color\": {\n          \"type\": \"string\"\n        },\n        \"size\": {\n          \"type\": \"string\"\n        },\n        \"weight\": {\n          \"type\": \"string\"\n        },\n        \"images\": {\n          \"type\": \"array\",\n          \"items\"\
  : {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          },\n          \"description\": \"Product image URLs.\"\n        },\n        \"stores\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"store_name\": {\"type\": \"string\"},\n              \"store_price\": {\"type\": \"string\"},\n              \"product_url\": {\"type\": \"string\", \"format\": \"uri\"}\n            }\n          },\n          \"description\": \"Retail store listings with prices.\"\n        }\n      },\n      \"required\": [\"title\"]\n    }\n  },\n  \"required\": [\"barcode_number\", \"barcode_type\", \"product\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/barcode-scanners/refs/heads/main/json-schema/barcode-lookup-schema.json
tags:
- Barcodes
- Inventory
- Product Lookup
- QR Codes
- Retail
- Scanning
- Supply Chain
title: BarcodeLookupResponse
---
