---
description: Response returned after successfully licensing a stock asset
layout: schema
name: LicenseResponse
properties_list:
- description: Content ID of the licensed asset
  name: content_id
  type: integer
- description: Details of the license purchase transaction
  name: purchase_details
  type: object
- description: URL to download the licensed full-resolution file
  name: download_url
  type: string
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-stock-license-response-schema.json
slug: adobe-creative-suite-stock-license-response
source_filename: adobe-creative-suite-stock-license-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-license-response-schema.json\",\n  \"title\": \"LicenseResponse\",\n  \"description\": \"Response returned after successfully licensing a stock asset\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Content ID of the licensed asset\",\n      \"example\": 123456789\n    },\n    \"purchase_details\": {\n      \"type\": \"object\",\n      \"description\": \"Details of the license purchase transaction\",\n      \"properties\": {\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"State of the license purchase\",\n          \"enum\": [\n            \"just_purchased\",\n            \"already_purchased\",\n            \"overage\"\n          ]\n        },\n        \"license\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"License type applied\"\n        },\n        \"nb_downloads\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of times this asset has been downloaded by the member\"\n        }\n      }\n    },\n    \"download_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to download the licensed full-resolution file\",\n      \"example\": \"https://stock.adobe.com/Rest/Libraries/Download/123456789/1\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-license-response-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: LicenseResponse
---
