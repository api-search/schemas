---
description: Dynamic response payload whose structure depends on the specific service and method invoked. Refer to the WADL for the deployed service.
layout: schema
name: ServiceMethodResponse
properties_list:
- description: Output parameters from the service method
  name: OutputParameters
  type: object
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/isg-rest-service-method-response-schema.json
slug: isg-rest-service-method-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceMethodResponse\",\n  \"type\": \"object\",\n  \"description\": \"Dynamic response payload whose structure depends on the specific service and method invoked. Refer to the WADL for the deployed service.\",\n  \"properties\": {\n    \"OutputParameters\": {\n      \"type\": \"object\",\n      \"description\": \"Output parameters from the service method\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/isg-rest-service-method-response-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: ServiceMethodResponse
---
