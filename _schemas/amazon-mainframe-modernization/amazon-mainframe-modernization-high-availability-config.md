---
description: Defines the details of a high availability configuration.
layout: schema
name: HighAvailabilityConfig
properties_list:
- description: ''
  name: desiredCapacity
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-high-availability-config-schema.json
slug: amazon-mainframe-modernization-high-availability-config
source_filename: amazon-mainframe-modernization-high-availability-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-high-availability-config-schema.json\",\n  \"title\": \"HighAvailabilityConfig\",\n  \"description\": \"Defines the details of a high availability configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"desiredCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CapacityValue\"\n        },\n        {\n          \"description\": \"The number of instances in a high availability configuration. The minimum possible value is 1 and the maximum is 100.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"desiredCapacity\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-high-availability-config-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: HighAvailabilityConfig
---
