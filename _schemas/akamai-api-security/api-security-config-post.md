---
description: Specifies the details of a security config.
layout: schema
name: config-post
properties_list:
- description: Contract ID.
  name: contractId
  type: string
- description: Contains details about a source configuration and version for cloning a new security configuration.
  name: createFrom
  type: object
- description: Describes the security configuration.
  name: description
  type: string
- description: Group ID.
  name: groupId
  type: integer
- description: List of hostnames to be added to the configuration.
  name: hostnames
  type: array
- description: The name you assigned to the security configuration.
  name: name
  type: string
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-config-post-schema.json
slug: api-security-config-post
source_filename: api-security-config-post-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-config-post-schema.json\",\n  \"title\": \"config-post\",\n  \"description\": \"Specifies the details of a security config.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contractId\": {\n      \"description\": \"Contract ID.\",\n      \"type\": \"string\"\n    },\n    \"createFrom\": {\n      \"additionalProperties\": false,\n      \"description\": \"Contains details about a source configuration and version for cloning a new security configuration.\",\n      \"properties\": {\n        \"configId\": {\n          \"description\": \"Uniquely identifies the security configuration.\",\n          \"type\": \"integer\"\n        },\n        \"version\": {\n          \"description\": \"The configuration version to clone from.\",\n          \"type\": \"integer\"\n        }\n      },\n\
  \      \"required\": [\n        \"configId\",\n        \"version\"\n      ],\n      \"type\": \"object\"\n    },\n    \"description\": {\n      \"description\": \"Describes the security configuration.\",\n      \"type\": \"string\"\n    },\n    \"groupId\": {\n      \"description\": \"Group ID.\",\n      \"type\": \"integer\"\n    },\n    \"hostnames\": {\n      \"description\": \"List of hostnames to be added to the configuration.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"name\": {\n      \"description\": \"The name you assigned to the security configuration.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"description\",\n    \"hostnames\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-config-post-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: config-post
---
