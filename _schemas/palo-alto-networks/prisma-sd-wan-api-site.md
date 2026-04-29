---
description: Site schema from Palo Alto Networks Prisma SD-WAN API
layout: schema
name: Site
properties_list:
- description: Unique identifier for the site.
  name: id
  type: string
- description: Name of the SD-WAN site.
  name: name
  type: string
- description: Optional description of the site.
  name: description
  type: string
- description: Administrative state of the site.
  name: admin_state
  type: string
- description: Role of the site in the SD-WAN topology.
  name: element_cluster_role
  type: string
- description: Physical address of the site.
  name: address
  type: object
- description: Geographic coordinates of the site.
  name: location
  type: object
- description: Tags for organizing and filtering sites.
  name: tags
  type: array
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-sd-wan-api-site-schema.json
slug: prisma-sd-wan-api-site
source_filename: prisma-sd-wan-api-site-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Site\",\n  \"description\": \"Site schema from Palo Alto Networks Prisma SD-WAN API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-sd-wan-api-site-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the site.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the SD-WAN site.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the site.\"\n    },\n    \"admin_state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"active\",\n        \"disabled\"\n      ],\n      \"default\": \"active\",\n      \"description\": \"Administrative state of the site.\"\n    },\n    \"element_cluster_role\"\
  : {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SPOKE\",\n        \"HUB\",\n        \"NONE\"\n      ],\n      \"default\": \"SPOKE\",\n      \"description\": \"Role of the site in the SD-WAN topology.\"\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"description\": \"Physical address of the site.\",\n      \"properties\": {\n        \"street\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"state\": {\n          \"type\": \"string\"\n        },\n        \"post_code\": {\n          \"type\": \"string\"\n        },\n        \"country\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"location\": {\n      \"type\": \"object\",\n      \"description\": \"Geographic coordinates of the site.\",\n      \"properties\": {\n        \"latitude\": {\n          \"type\": \"number\",\n          \"format\": \"double\"\n        },\n        \"longitude\": {\n          \"type\"\
  : \"number\",\n          \"format\": \"double\"\n        }\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags for organizing and filtering sites.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-sd-wan-api-site-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Site
---
