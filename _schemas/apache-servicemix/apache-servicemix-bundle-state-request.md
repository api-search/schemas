---
description: Request to update bundle state
layout: schema
name: BundleStateRequest
properties_list:
- description: Target state action
  name: state
  type: string
provider_name: Apache ServiceMix
provider_slug: apache-servicemix
schema_file: json-schema/apache-servicemix-bundle-state-request-schema.json
slug: apache-servicemix-bundle-state-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-servicemix/refs/heads/main/json-schema/apache-servicemix-bundle-state-request-schema.json\",\n  \"title\": \"BundleStateRequest\",\n  \"description\": \"Request to update bundle state\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"start\",\n        \"stop\",\n        \"restart\",\n        \"refresh\",\n        \"update\"\n      ],\n      \"description\": \"Target state action\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-servicemix/refs/heads/main/json-schema/apache-servicemix-bundle-state-request-schema.json
tags:
- Enterprise Integration
- ESB
- Integration
- Messaging
- OSGi
- Apache
- Open Source
title: BundleStateRequest
---
