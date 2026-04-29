---
description: The connection between two service in an insight impact graph.
layout: schema
name: InsightImpactGraphEdge
properties_list:
- description: ''
  name: ReferenceId
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-insight-impact-graph-edge-schema.json
slug: xray-insight-impact-graph-edge
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReferenceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"Identifier of the edge. Unique within a service map.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The connection between two service in an insight impact graph.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InsightImpactGraphEdge\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-insight-impact-graph-edge-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-insight-impact-graph-edge-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: InsightImpactGraphEdge
---
