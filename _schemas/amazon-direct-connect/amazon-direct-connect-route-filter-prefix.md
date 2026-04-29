---
description: Information about a route filter prefix that a customer can advertise through Border Gateway Protocol (BGP) over a public virtual interface.
layout: schema
name: RouteFilterPrefix
properties_list:
- description: ''
  name: cidr
  type: object
provider_name: Amazon Direct Connect
provider_slug: amazon-direct-connect
schema_file: json-schema/amazon-direct-connect-route-filter-prefix-schema.json
slug: amazon-direct-connect-route-filter-prefix
source_filename: amazon-direct-connect-route-filter-prefix-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-route-filter-prefix-schema.json\",\n  \"title\": \"RouteFilterPrefix\",\n  \"description\": \"Information about a route filter prefix that a customer can advertise through Border Gateway Protocol (BGP) over a public virtual interface.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cidr\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CIDR\"\n        },\n        {\n          \"description\": \"The CIDR block for the advertised route. Separate multiple routes using commas. An IPv6 CIDR must use /64 or shorter.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-route-filter-prefix-schema.json
tags:
- AWS
- Dedicated Connection
- Direct Connect
- Hybrid Cloud
- Networking
title: RouteFilterPrefix
---
