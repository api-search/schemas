---
description: Dynamic request payload whose structure depends on the specific service and method being invoked. Refer to the WADL for the deployed service.
layout: schema
name: ServiceMethodRequest
properties_list:
- description: Optional REST header for overriding application context on a per-request basis. Only required if the context differs from the initialized session.
  name: RESTHeader
  type: object
- description: Input parameters specific to the service method. Structure varies by service - consult the WADL.
  name: InputParameters
  type: object
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/isg-rest-service-method-request-schema.json
slug: isg-rest-service-method-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceMethodRequest\",\n  \"type\": \"object\",\n  \"description\": \"Dynamic request payload whose structure depends on the specific service and method being invoked. Refer to the WADL for the deployed service.\",\n  \"properties\": {\n    \"RESTHeader\": {\n      \"type\": \"object\",\n      \"description\": \"Optional REST header for overriding application context on a per-request basis. Only required if the context differs from the initialized session.\"\n    },\n    \"InputParameters\": {\n      \"type\": \"object\",\n      \"description\": \"Input parameters specific to the service method. Structure varies by service - consult the WADL.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/isg-rest-service-method-request-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: ServiceMethodRequest
---
