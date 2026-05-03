---
description: Named slots available in the rapi-doc web component where custom HTML content can be injected at predefined locations within the documentation UI.
layout: schema
name: RapiDoc Slots
properties_list:
- description: Slot for a custom logo image displayed in the navigation header.
  name: logo
  type: string
- description: Slot for custom header content placed in the header bar area.
  name: header
  type: string
- description: Slot for custom footer content placed at the bottom of the documentation.
  name: footer
  type: string
- description: Slot for a custom logo in the navigation sidebar.
  name: nav-logo
  type: string
- description: Slot for custom content displayed in the API overview/info section.
  name: overview
  type: string
- description: Slot for custom content in the servers section.
  name: servers
  type: string
- description: Slot for custom content in the authentication section.
  name: auth
  type: string
- description: Dynamic slot for injecting custom content before a specific tag group, where {tag-name} is the tag's name in lowercase with spaces replaced by hyphens.
  name: tag--{tag-name}
  type: string
- description: Dynamic slot for injecting custom content before a specific endpoint.
  name: endpoint--{method}--{path}
  type: string
provider_name: RapiDoc
provider_slug: rapidoc
schema_file: json-schema/rapidoc-slots.json
slug: rapidoc-slots
source_filename: rapidoc-slots.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/rapidoc/blob/main/json-schema/rapidoc-slots.json\",\n  \"title\": \"RapiDoc Slots\",\n  \"description\": \"Named slots available in the rapi-doc web component where custom HTML content can be injected at predefined locations within the documentation UI.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"logo\": {\n      \"type\": \"string\",\n      \"description\": \"Slot for a custom logo image displayed in the navigation header.\"\n    },\n    \"header\": {\n      \"type\": \"string\",\n      \"description\": \"Slot for custom header content placed in the header bar area.\"\n    },\n    \"footer\": {\n      \"type\": \"string\",\n      \"description\": \"Slot for custom footer content placed at the bottom of the documentation.\"\n    },\n    \"nav-logo\": {\n      \"type\": \"string\",\n      \"description\": \"Slot for a custom logo in the navigation sidebar.\"\
  \n    },\n    \"overview\": {\n      \"type\": \"string\",\n      \"description\": \"Slot for custom content displayed in the API overview/info section.\"\n    },\n    \"servers\": {\n      \"type\": \"string\",\n      \"description\": \"Slot for custom content in the servers section.\"\n    },\n    \"auth\": {\n      \"type\": \"string\",\n      \"description\": \"Slot for custom content in the authentication section.\"\n    },\n    \"tag--{tag-name}\": {\n      \"type\": \"string\",\n      \"description\": \"Dynamic slot for injecting custom content before a specific tag group, where {tag-name} is the tag's name in lowercase with spaces replaced by hyphens.\"\n    },\n    \"endpoint--{method}--{path}\": {\n      \"type\": \"string\",\n      \"description\": \"Dynamic slot for injecting custom content before a specific endpoint.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rapidoc/refs/heads/main/json-schema/rapidoc-slots.json
tags:
- Documentation
- Platform
- Web Components
- OpenAPI
title: RapiDoc Slots
---
