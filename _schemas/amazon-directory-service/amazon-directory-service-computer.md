---
description: Contains information about a computer account in a directory.
layout: schema
name: Computer
properties_list:
- description: ''
  name: ComputerId
  type: object
- description: ''
  name: ComputerName
  type: object
- description: ''
  name: ComputerAttributes
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-computer-schema.json
slug: amazon-directory-service-computer
source_filename: amazon-directory-service-computer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-computer-schema.json\",\n  \"title\": \"Computer\",\n  \"description\": \"Contains information about a computer account in a directory.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ComputerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SID\"\n        },\n        {\n          \"description\": \"The identifier of the computer.\"\n        }\n      ]\n    },\n    \"ComputerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputerName\"\n        },\n        {\n          \"description\": \"The computer name.\"\n        }\n      ]\n    },\n    \"ComputerAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Attributes\"\n        },\n        {\n          \"description\"\
  : \"An array of <a>Attribute</a> objects containing the LDAP attributes that belong to the computer account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-computer-schema.json
tags:
- Active Directory
- Authentication
- Directory Services
- Identity Management
title: Computer
---
