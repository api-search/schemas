---
description: A name value pair that Image Builder applies to streamline results from the vulnerability scan findings list action.
layout: schema
name: ImageScanFindingsFilter
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: values
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-image-scan-findings-filter-schema.json
slug: ec2-image-builder-image-scan-findings-filter
source_filename: ec2-image-builder-image-scan-findings-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-scan-findings-filter-schema.json\",\n  \"title\": \"ImageScanFindingsFilter\",\n  \"description\": \"A name value pair that Image Builder applies to streamline results from the vulnerability scan findings list action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterName\"\n        },\n        {\n          \"description\": \"The name of the image scan finding filter. Filter names are case-sensitive.\"\n        }\n      ]\n    },\n    \"values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageScanFindingsFilterValues\"\n        },\n        {\n          \"description\": \"The filter values. Filter values are case-sensitive.\"\n        }\n  \
  \    ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-scan-findings-filter-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ImageScanFindingsFilter
---
