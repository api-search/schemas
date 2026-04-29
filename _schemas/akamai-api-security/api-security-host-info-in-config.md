---
description: Contains the list of hostnames available for protection and its details.
layout: schema
name: host-info-in-config
properties_list:
- description: The available hosts set for the current user.
  name: availableSet
  type: array
- description: Uniquely identifies the security configuration.
  name: configId
  type: integer
- description: The security configuration version.
  name: configVersion
  type: integer
- description: The requested hosts aren't available in this configuration version.
  name: errorSet
  type: array
- description: Whether the host defined in the ARL file has legacy WAF enabled in the configuration.
  name: protectARLInclusionHost
  type: boolean
- description: The selected set of hostnames in this configuration version.
  name: selectedSet
  type: array
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-host-info-in-config-schema.json
slug: api-security-host-info-in-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-host-info-in-config-schema.json\",\n  \"title\": \"host-info-in-config\",\n  \"description\": \"Contains the list of hostnames available for protection and its details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"availableSet\": {\n      \"description\": \"The available hosts set for the current user.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"description\": \"Contains details about the hostname and its status.\",\n        \"properties\": {\n          \"activeInProduction\": {\n            \"description\": \"Whether the hostname is active in the production network.\",\n            \"type\": \"boolean\"\n          },\n          \"activeInStaging\": {\n            \"description\": \"Whether the hostname is active in the staging network.\",\n \
  \           \"type\": \"boolean\"\n          },\n          \"arlInclusion\": {\n            \"description\": \"Whether the hostname is Akamai Resource Locator (ARL) included.\",\n            \"type\": \"boolean\"\n          },\n          \"configIdInProduction\": {\n            \"description\": \"Uniquely identifies the configuration that protects the hostname.\",\n            \"nullable\": true,\n            \"type\": \"integer\"\n          },\n          \"configNameInProduction\": {\n            \"description\": \"The name of the configuration that protects the hostname.\",\n            \"nullable\": true,\n            \"type\": \"string\"\n          },\n          \"hostname\": {\n            \"description\": \"The hostname.\",\n            \"type\": \"string\"\n          }\n        },\n        \"required\": [\n          \"hostname\"\n        ],\n        \"type\": \"object\",\n        \"x-akamai\": {\n          \"file-path\": \"schemas/hostname-object.yaml\"\n        }\n      },\n  \
  \    \"type\": \"array\"\n    },\n    \"configId\": {\n      \"description\": \"Uniquely identifies the security configuration.\",\n      \"type\": \"integer\"\n    },\n    \"configVersion\": {\n      \"description\": \"The security configuration version.\",\n      \"type\": \"integer\"\n    },\n    \"errorSet\": {\n      \"description\": \"The requested hosts aren't available in this configuration version.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"properties\": {\n          \"hostname\": {\n            \"description\": \"The hostname that triggers an error.\",\n            \"type\": \"string\"\n          },\n          \"reason\": {\n            \"description\": \"The reason why the hosts aren't protectable in this configuration version.\",\n            \"type\": \"string\"\n          },\n          \"reasonCode\": {\n            \"description\": \"The error status code for the hostname.\",\n            \"type\": \"integer\"\n          }\n        },\n \
  \       \"required\": [\n          \"reason\",\n          \"reasonCode\",\n          \"hostname\"\n        ],\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    },\n    \"protectARLInclusionHost\": {\n      \"description\": \"Whether the host defined in the ARL file has legacy WAF enabled in the configuration.\",\n      \"type\": \"boolean\"\n    },\n    \"selectedSet\": {\n      \"description\": \"The selected set of hostnames in this configuration version.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"description\": \"Contains details about the hostname and its status.\",\n        \"properties\": {\n          \"activeInProduction\": {\n            \"description\": \"Whether the hostname is active in the production network.\",\n            \"type\": \"boolean\"\n          },\n          \"activeInStaging\": {\n            \"description\": \"Whether the hostname is active in the staging network.\",\n            \"type\": \"boolean\"\n \
  \         },\n          \"arlInclusion\": {\n            \"description\": \"Whether the hostname is Akamai Resource Locator (ARL) included.\",\n            \"type\": \"boolean\"\n          },\n          \"configIdInProduction\": {\n            \"description\": \"Uniquely identifies the configuration that protects the hostname.\",\n            \"nullable\": true,\n            \"type\": \"integer\"\n          },\n          \"configNameInProduction\": {\n            \"description\": \"The name of the configuration that protects the hostname.\",\n            \"nullable\": true,\n            \"type\": \"string\"\n          },\n          \"hostname\": {\n            \"description\": \"The hostname.\",\n            \"type\": \"string\"\n          }\n        },\n        \"required\": [\n          \"hostname\"\n        ],\n        \"type\": \"object\",\n        \"x-akamai\": {\n          \"file-path\": \"schemas/hostname-object.yaml\"\n        }\n      },\n      \"type\": \"array\"\n    }\n  },\n\
  \  \"required\": [\n    \"configId\",\n    \"configVersion\",\n    \"protectARLInclusionHost\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-host-info-in-config-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: host-info-in-config
---
