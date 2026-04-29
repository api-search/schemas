---
description: An Ambassador Mapping resource that associates a URL prefix or path with a backend service. Mappings are the primary mechanism for configuring routing in Ambassador Edge Stack.
layout: schema
name: Mapping
properties_list:
- description: API version for the Mapping resource
  name: apiVersion
  type: string
- description: Resource kind
  name: kind
  type: string
provider_name: Ambassador
provider_slug: ambassador
schema_file: json-schema/ambassador-mapping-schema.json
slug: ambassador-mapping
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Mapping\",\n  \"type\": \"object\",\n  \"description\": \"An Ambassador Mapping resource that associates a URL prefix or path with a backend service. Mappings are the primary mechanism for configuring routing in Ambassador Edge Stack.\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"description\": \"API version for the Mapping resource\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Resource kind\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/json-schema/ambassador-mapping-schema.json
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
title: Mapping
---
