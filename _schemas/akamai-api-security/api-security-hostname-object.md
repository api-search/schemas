---
description: Contains details about the hostname and its status.
layout: schema
name: hostname-object
properties_list:
- description: Whether the hostname is active in the production network.
  name: activeInProduction
  type: boolean
- description: Whether the hostname is active in the staging network.
  name: activeInStaging
  type: boolean
- description: Whether the hostname is Akamai Resource Locator (ARL) included.
  name: arlInclusion
  type: boolean
- description: Uniquely identifies the configuration that protects the hostname.
  name: configIdInProduction
  type: integer
- description: The name of the configuration that protects the hostname.
  name: configNameInProduction
  type: string
- description: The hostname.
  name: hostname
  type: string
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-hostname-object-schema.json
slug: api-security-hostname-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-hostname-object-schema.json\",\n  \"title\": \"hostname-object\",\n  \"description\": \"Contains details about the hostname and its status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"activeInProduction\": {\n      \"description\": \"Whether the hostname is active in the production network.\",\n      \"type\": \"boolean\"\n    },\n    \"activeInStaging\": {\n      \"description\": \"Whether the hostname is active in the staging network.\",\n      \"type\": \"boolean\"\n    },\n    \"arlInclusion\": {\n      \"description\": \"Whether the hostname is Akamai Resource Locator (ARL) included.\",\n      \"type\": \"boolean\"\n    },\n    \"configIdInProduction\": {\n      \"description\": \"Uniquely identifies the configuration that protects the hostname.\",\n      \"nullable\"\
  : true,\n      \"type\": \"integer\"\n    },\n    \"configNameInProduction\": {\n      \"description\": \"The name of the configuration that protects the hostname.\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"hostname\": {\n      \"description\": \"The hostname.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"hostname\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-hostname-object-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: hostname-object
---
