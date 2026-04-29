---
description: Specifies the details of a security config.
layout: schema
name: configs-get
properties_list:
- description: A list of security configurations.
  name: configurations
  type: array
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-configs-get-schema.json
slug: api-security-configs-get
source_filename: api-security-configs-get-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-configs-get-schema.json\",\n  \"title\": \"configs-get\",\n  \"description\": \"Specifies the details of a security config.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configurations\": {\n      \"description\": \"A list of security configurations.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"description\": \"Contains details about a security configuration.\",\n        \"properties\": {\n          \"description\": {\n            \"description\": \"__Read-only__ Describes the security configuration.\",\n            \"readOnly\": true,\n            \"type\": \"string\"\n          },\n          \"id\": {\n            \"description\": \"__Read-only__ Uniquely identifies the security configuration.\",\n            \"readOnly\": true,\n            \"\
  type\": \"integer\"\n          },\n          \"latestVersion\": {\n            \"description\": \"__Read-only__ The latest version of the security configuration.\",\n            \"readOnly\": true,\n            \"type\": \"integer\"\n          },\n          \"name\": {\n            \"description\": \"__Read-only__ The security configuration name.\",\n            \"readOnly\": true,\n            \"type\": \"string\"\n          },\n          \"productionHostnames\": {\n            \"description\": \"__Read-only__ The list of hostnames protected by this security configuration in the production network.\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"readOnly\": true,\n            \"type\": \"array\"\n          },\n          \"productionVersion\": {\n            \"description\": \"__Read-only__ The latest security configuration version active in the production network.\",\n            \"readOnly\": true,\n            \"type\": \"integer\"\n \
  \         },\n          \"stagingVersion\": {\n            \"description\": \"__Read-only__ The latest security configuration version active in the staging network.\",\n            \"readOnly\": true,\n            \"type\": \"integer\"\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"latestVersion\",\n          \"name\"\n        ],\n        \"type\": \"object\",\n        \"x-akamai\": {\n          \"file-path\": \"schemas/config-get.yaml\"\n        }\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"configurations\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-configs-get-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: configs-get
---
