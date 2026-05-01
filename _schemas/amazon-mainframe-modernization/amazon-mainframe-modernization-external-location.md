---
description: Defines an external storage location.
layout: schema
name: ExternalLocation
properties_list:
- description: ''
  name: s3Location
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-external-location-schema.json
slug: amazon-mainframe-modernization-external-location
source_filename: amazon-mainframe-modernization-external-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-external-location-schema.json\",\n  \"title\": \"ExternalLocation\",\n  \"description\": \"Defines an external storage location.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String2000\"\n        },\n        {\n          \"description\": \"The URI of the Amazon S3 bucket.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-external-location-schema.json
tags:
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: ExternalLocation
---
