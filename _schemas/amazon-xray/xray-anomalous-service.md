---
description: The service within the service graph that has anomalously high fault rates.
layout: schema
name: AnomalousService
properties_list:
- description: ''
  name: ServiceId
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-anomalous-service-schema.json
slug: xray-anomalous-service
source_filename: xray-anomalous-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceId\": {\n      \"$ref\": \"#/components/schemas/ServiceId\"\n    }\n  },\n  \"description\": \"The service within the service graph that has anomalously high fault rates. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AnomalousService\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-anomalous-service-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-anomalous-service-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: AnomalousService
---
