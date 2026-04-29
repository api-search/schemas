---
description: AttributeMap schema from Amazon X-Ray API
layout: schema
name: AttributeMap
properties_list: []
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-attribute-map-schema.json
slug: xray-attribute-map
source_json: "{\n  \"type\": \"object\",\n  \"maxProperties\": 5,\n  \"additionalProperties\": {\n    \"$ref\": \"#/components/schemas/AttributeValue\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AttributeMap\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-attribute-map-schema.json\",\n  \"description\": \"AttributeMap schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-attribute-map-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: AttributeMap
---
