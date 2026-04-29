---
description: Contains details about a security configuration.
layout: schema
name: config-get
properties_list:
- description: __Read-only__ Describes the security configuration.
  name: description
  type: string
- description: __Read-only__ Uniquely identifies the security configuration.
  name: id
  type: integer
- description: __Read-only__ The latest version of the security configuration.
  name: latestVersion
  type: integer
- description: __Read-only__ The security configuration name.
  name: name
  type: string
- description: __Read-only__ The list of hostnames protected by this security configuration in the production network.
  name: productionHostnames
  type: array
- description: __Read-only__ The latest security configuration version active in the production network.
  name: productionVersion
  type: integer
- description: __Read-only__ The latest security configuration version active in the staging network.
  name: stagingVersion
  type: integer
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-config-get-schema.json
slug: api-security-config-get
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-config-get-schema.json\",\n  \"title\": \"config-get\",\n  \"description\": \"Contains details about a security configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"__Read-only__ Describes the security configuration.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"__Read-only__ Uniquely identifies the security configuration.\",\n      \"readOnly\": true,\n      \"type\": \"integer\"\n    },\n    \"latestVersion\": {\n      \"description\": \"__Read-only__ The latest version of the security configuration.\",\n      \"readOnly\": true,\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"description\": \"__Read-only__ The security configuration name.\",\n    \
  \  \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"productionHostnames\": {\n      \"description\": \"__Read-only__ The list of hostnames protected by this security configuration in the production network.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"productionVersion\": {\n      \"description\": \"__Read-only__ The latest security configuration version active in the production network.\",\n      \"readOnly\": true,\n      \"type\": \"integer\"\n    },\n    \"stagingVersion\": {\n      \"description\": \"__Read-only__ The latest security configuration version active in the staging network.\",\n      \"readOnly\": true,\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"latestVersion\",\n    \"name\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-config-get-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: config-get
---
