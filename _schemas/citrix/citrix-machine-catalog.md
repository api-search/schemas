---
description: A machine catalog defines a collection of virtual or physical machines managed as a single entity for provisioning in Citrix DaaS or Virtual Apps and Desktops.
layout: schema
name: Citrix Machine Catalog
properties_list:
- description: Unique identifier for the machine catalog
  name: id
  type: string
- description: Name of the machine catalog
  name: name
  type: string
- description: Description of the machine catalog
  name: description
  type: string
- description: How machines are allocated to users
  name: allocationType
  type: string
- description: Provisioning method for machines in the catalog
  name: provisioningType
  type: string
- description: Whether machines support single or multiple concurrent sessions
  name: sessionSupport
  type: string
- description: Number of machines in the catalog
  name: machineCount
  type: integer
- description: ''
  name: zone
  type: object
provider_name: Citrix
provider_slug: citrix
schema_file: json-schema/citrix-machine-catalog-schema.json
slug: citrix-machine-catalog
source_filename: citrix-machine-catalog-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.citrix.com/schemas/citrix/machine-catalog.json\",\n  \"title\": \"Citrix Machine Catalog\",\n  \"description\": \"A machine catalog defines a collection of virtual or physical machines managed as a single entity for provisioning in Citrix DaaS or Virtual Apps and Desktops.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"allocationType\", \"provisioningType\", \"sessionSupport\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the machine catalog\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the machine catalog\",\n      \"minLength\": 1,\n      \"maxLength\": 256\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the machine catalog\"\n    },\n    \"allocationType\": {\n      \"type\": \"string\",\n      \"\
  enum\": [\"Static\", \"Random\"],\n      \"description\": \"How machines are allocated to users\"\n    },\n    \"provisioningType\": {\n      \"type\": \"string\",\n      \"enum\": [\"MCS\", \"PVS\", \"Manual\"],\n      \"description\": \"Provisioning method for machines in the catalog\"\n    },\n    \"sessionSupport\": {\n      \"type\": \"string\",\n      \"enum\": [\"SingleSession\", \"MultiSession\"],\n      \"description\": \"Whether machines support single or multiple concurrent sessions\"\n    },\n    \"machineCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of machines in the catalog\"\n    },\n    \"zone\": {\n      \"$ref\": \"#/$defs/Zone\"\n    }\n  },\n  \"$defs\": {\n    \"Zone\": {\n      \"type\": \"object\",\n      \"description\": \"Resource zone where the catalog is hosted\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Zone unique identifier\"\n        },\n\
  \        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Zone display name\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/citrix/refs/heads/main/json-schema/citrix-machine-catalog-schema.json
tags:
- Application Delivery
- Desktop-As-A-Service
- Networking
- Virtualization
- Workspace
title: Citrix Machine Catalog
---
