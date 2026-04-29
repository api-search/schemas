---
description: OSGi bundle in ServiceMix
layout: schema
name: Bundle
properties_list:
- description: Bundle identifier
  name: id
  type: integer
- description: Bundle name
  name: name
  type: string
- description: Bundle symbolic name
  name: symbolicName
  type: string
- description: Bundle version
  name: version
  type: string
- description: Bundle state
  name: state
  type: string
- description: Bundle location URL
  name: location
  type: string
provider_name: Apache ServiceMix
provider_slug: apache-servicemix
schema_file: json-schema/apache-servicemix-bundle-schema.json
slug: apache-servicemix-bundle
source_filename: apache-servicemix-bundle-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-servicemix/refs/heads/main/json-schema/apache-servicemix-bundle-schema.json\",\n  \"title\": \"Bundle\",\n  \"description\": \"OSGi bundle in ServiceMix\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Bundle identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Bundle name\"\n    },\n    \"symbolicName\": {\n      \"type\": \"string\",\n      \"description\": \"Bundle symbolic name\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Bundle version\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"INSTALLED\",\n        \"RESOLVED\",\n        \"STARTING\",\n        \"ACTIVE\",\n        \"STOPPING\",\n        \"UNINSTALLED\"\n      ],\n      \"description\": \"Bundle\
  \ state\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Bundle location URL\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-servicemix/refs/heads/main/json-schema/apache-servicemix-bundle-schema.json
tags:
- Enterprise Integration
- ESB
- Integration
- Messaging
- OSGi
- Apache
- Open Source
title: Bundle
---
