---
description: Name of the availability zone.
layout: schema
name: AvailabilityZone
properties_list:
- description: ''
  name: Name
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-availability-zone-schema.json
slug: mq-api-availability-zone
source_filename: mq-api-availability-zone-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-availability-zone-schema.json\",\n  \"title\": \"AvailabilityZone\",\n  \"description\": \"Name of the availability zone.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Id for the availability zone.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-availability-zone-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: AvailabilityZone
---
