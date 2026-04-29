---
description: List of OSGi bundles
layout: schema
name: BundleList
properties_list:
- description: ''
  name: bundles
  type: array
- description: ''
  name: total
  type: integer
provider_name: Apache ServiceMix
provider_slug: apache-servicemix
schema_file: json-schema/apache-servicemix-bundle-list-schema.json
slug: apache-servicemix-bundle-list
source_filename: apache-servicemix-bundle-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-servicemix/refs/heads/main/json-schema/apache-servicemix-bundle-list-schema.json\",\n  \"title\": \"BundleList\",\n  \"description\": \"List of OSGi bundles\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bundles\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Bundle\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-servicemix/refs/heads/main/json-schema/apache-servicemix-bundle-list-schema.json
tags:
- Enterprise Integration
- ESB
- Integration
- Messaging
- OSGi
- Apache
- Open Source
title: BundleList
---
