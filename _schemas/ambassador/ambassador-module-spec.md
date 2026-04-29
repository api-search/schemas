---
description: Specification for a Module resource
layout: schema
name: ModuleSpec
properties_list:
- description: Module configuration. The shape depends on the module name (e.g., ambassador, authentication, tracing).
  name: config
  type: object
- description: Ambassador IDs that should apply this Module
  name: ambassador_id
  type: array
provider_name: Ambassador
provider_slug: ambassador
schema_file: json-schema/ambassador-module-spec-schema.json
slug: ambassador-module-spec
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ModuleSpec\",\n  \"type\": \"object\",\n  \"description\": \"Specification for a Module resource\",\n  \"properties\": {\n    \"config\": {\n      \"type\": \"object\",\n      \"description\": \"Module configuration. The shape depends on the module name (e.g., ambassador, authentication, tracing).\"\n    },\n    \"ambassador_id\": {\n      \"type\": \"array\",\n      \"description\": \"Ambassador IDs that should apply this Module\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/json-schema/ambassador-module-spec-schema.json
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
title: ModuleSpec
---
