---
description: Contains configuration version details.
layout: schema
name: waf-config-version
properties_list:
- description: __Read-only__ The version from which you cloned this version.
  name: basedOn
  type: integer
- description: __Read-only__ Uniquely identifies the security configuration.
  name: configId
  type: integer
- description: The security configuration name.
  name: configName
  type: string
- description: __Read-only__ The date when you created the configuration version.
  name: createDate
  type: string
- description: __Read-only__ The user who created the configuration version.
  name: createdBy
  type: string
- description: __Read-only__ The activation status of the configuration version in the production network.
  name: production
  type: object
- description: __Read-only__ The activation status of the configuration version in the staging network.
  name: staging
  type: object
- description: __Read-only__ The security configuration version.
  name: version
  type: integer
- description: The notes you entered for the configuration version.
  name: versionNotes
  type: string
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-waf-config-version-schema.json
slug: api-security-waf-config-version
source_filename: api-security-waf-config-version-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-waf-config-version-schema.json\",\n  \"title\": \"waf-config-version\",\n  \"description\": \"Contains configuration version details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"basedOn\": {\n      \"description\": \"__Read-only__ The version from which you cloned this version.\",\n      \"readOnly\": true,\n      \"type\": \"integer\"\n    },\n    \"configId\": {\n      \"description\": \"__Read-only__ Uniquely identifies the security configuration.\",\n      \"readOnly\": true,\n      \"type\": \"integer\"\n    },\n    \"configName\": {\n      \"description\": \"The security configuration name.\",\n      \"type\": \"string\"\n    },\n    \"createDate\": {\n      \"description\": \"__Read-only__ The date when you created the configuration version.\",\n      \"readOnly\": true,\n\
  \      \"type\": \"string\"\n    },\n    \"createdBy\": {\n      \"description\": \"__Read-only__ The user who created the configuration version.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"production\": {\n      \"additionalProperties\": false,\n      \"description\": \"__Read-only__ The activation status of the configuration version in the production network.\",\n      \"properties\": {\n        \"action\": {\n          \"description\": \"The action taken on the configuration version. Either `ACTIVATE` or `DEACTIVATE`.\",\n          \"enum\": [\n            \"ACTIVATE\",\n            \"DEACTIVATE\"\n          ],\n          \"type\": \"string\"\n        },\n        \"status\": {\n          \"description\": \"The activation status, either `Pending`, `Active`, `Inactive`, `Deactivated`, or `Failed`.\",\n          \"enum\": [\n            \"Pending\",\n            \"Active\",\n            \"Inactive\",\n            \"Deactivated\",\n            \"Failed\"\n \
  \         ],\n          \"type\": \"string\"\n        },\n        \"time\": {\n          \"description\": \"The activation time.\",\n          \"type\": \"string\"\n        }\n      },\n      \"readOnly\": true,\n      \"required\": [\n        \"status\"\n      ],\n      \"type\": \"object\"\n    },\n    \"staging\": {\n      \"additionalProperties\": false,\n      \"description\": \"__Read-only__ The activation status of the configuration version in the staging network.\",\n      \"properties\": {\n        \"action\": {\n          \"description\": \"The action taken on the configuration version. Either `ACTIVATE` or `DEACTIVATE`.\",\n          \"enum\": [\n            \"ACTIVATE\",\n            \"DEACTIVATE\"\n          ],\n          \"type\": \"string\"\n        },\n        \"status\": {\n          \"description\": \"The activation status, either `Pending`, `Active`, `Inactive`, `Deactivated`, or `Failed`.\",\n          \"enum\": [\n            \"Pending\",\n            \"Active\",\n\
  \            \"Inactive\",\n            \"Deactivated\",\n            \"Failed\"\n          ],\n          \"type\": \"string\"\n        },\n        \"time\": {\n          \"description\": \"The ISO 8601 time stamp indicating the activation time.\",\n          \"type\": \"string\"\n        }\n      },\n      \"readOnly\": true,\n      \"required\": [\n        \"status\"\n      ],\n      \"type\": \"object\"\n    },\n    \"version\": {\n      \"description\": \"__Read-only__ The security configuration version.\",\n      \"readOnly\": true,\n      \"type\": \"integer\"\n    },\n    \"versionNotes\": {\n      \"description\": \"The notes you entered for the configuration version.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"configId\",\n    \"configName\",\n    \"version\",\n    \"staging\",\n    \"production\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-waf-config-version-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: waf-config-version
---
