---
description: An object that represents the egress filter rules for a service mesh.
layout: schema
name: EgressFilter
properties_list:
- description: ''
  name: type
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-egress-filter-schema.json
slug: app-mesh-egress-filter
source_filename: app-mesh-egress-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EgressFilterType\"\n        },\n        {\n          \"description\": \"The egress filter type. By default, the type is <code>DROP_ALL</code>, which allows egress only from virtual nodes to other defined resources in the service mesh (and any traffic to <code>*.amazonaws.com</code> for Amazon Web Services API calls). You can set the egress filter type to <code>ALLOW_ALL</code> to allow egress to any endpoint inside or outside of the service mesh.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"type\"\n  ],\n  \"description\": \"An object that represents the egress filter rules for a service mesh.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-egress-filter-schema.json\",\n  \"title\": \"EgressFilter\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-egress-filter-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: EgressFilter
---
