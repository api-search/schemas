---
description: A list of Availability Zones corresponding to the segments in a trace.
layout: schema
name: AvailabilityZoneDetail
properties_list:
- description: ''
  name: Name
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-availability-zone-detail-schema.json
slug: xray-availability-zone-detail
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of a corresponding Availability Zone.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A list of Availability Zones corresponding to the segments in a trace.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AvailabilityZoneDetail\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-availability-zone-detail-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-availability-zone-detail-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: AvailabilityZoneDetail
---
