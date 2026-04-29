---
description: Contains a key range. For export jobs, a <code>S3Resource</code> object can have an optional <code>KeyRange</code> value. The length of the range is defined at job creation, and has either an inclusive <code>BeginMarker</code>, an inclusive <code>EndMarker</code>, or both. Ranges are UTF-8 binary sorted.
layout: schema
name: KeyRange
properties_list:
- description: ''
  name: BeginMarker
  type: object
- description: ''
  name: EndMarker
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-key-range-schema.json
slug: amazon-snow-family-key-range
source_filename: amazon-snow-family-key-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-key-range-schema.json\",\n  \"title\": \"KeyRange\",\n  \"description\": \"Contains a key range. For export jobs, a <code>S3Resource</code> object can have an optional <code>KeyRange</code> value. The length of the range is defined at job creation, and has either an inclusive <code>BeginMarker</code>, an inclusive <code>EndMarker</code>, or both. Ranges are UTF-8 binary sorted.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BeginMarker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The key that starts an optional key range for an export job. Ranges are inclusive and UTF-8 binary sorted.\"\n        }\n      ]\n    },\n    \"EndMarker\": {\n      \"allOf\": [\n        {\n        \
  \  \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The key that ends an optional key range for an export job. Ranges are inclusive and UTF-8 binary sorted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-key-range-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: KeyRange
---
