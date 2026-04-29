---
description: Contains details about a security configuration's versions.
layout: schema
name: waf-config-versions
properties_list:
- description: Uniquely identifies the security configuration.
  name: configId
  type: integer
- description: The name you assigned to the security configuration.
  name: configName
  type: string
- description: The version number of the security configuration that you created most recently.
  name: lastCreatedVersion
  type: integer
- description: The current page number.
  name: page
  type: integer
- description: Represents the number of items per page.
  name: pageSize
  type: integer
- description: The version number of the security configuration that is currently active on the production network.
  name: productionActiveVersion
  type: integer
- description: Uniquely identifies the expedite activation request of the configuration version on the production network.
  name: productionExpediteRequestId
  type: integer
- description: The version number of the security configuration that is currently active on the staging network.
  name: stagingActiveVersion
  type: integer
- description: Uniquely identifies the expedite activation request of the configuration version on the staging network.
  name: stagingExpediteRequestId
  type: integer
- description: The total number of configuration versions.
  name: totalSize
  type: integer
- description: The security configuration's versions.
  name: versionList
  type: array
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-waf-config-versions-schema.json
slug: api-security-waf-config-versions
source_filename: api-security-waf-config-versions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-waf-config-versions-schema.json\",\n  \"title\": \"waf-config-versions\",\n  \"description\": \"Contains details about a security configuration's versions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configId\": {\n      \"description\": \"Uniquely identifies the security configuration.\",\n      \"type\": \"integer\"\n    },\n    \"configName\": {\n      \"description\": \"The name you assigned to the security configuration.\",\n      \"type\": \"string\"\n    },\n    \"lastCreatedVersion\": {\n      \"description\": \"The version number of the security configuration that you created most recently.\",\n      \"type\": \"integer\"\n    },\n    \"page\": {\n      \"description\": \"The current page number.\",\n      \"type\": \"integer\"\n    },\n    \"pageSize\": {\n      \"\
  description\": \"Represents the number of items per page.\",\n      \"type\": \"integer\"\n    },\n    \"productionActiveVersion\": {\n      \"description\": \"The version number of the security configuration that is currently active on the production network.\",\n      \"type\": \"integer\"\n    },\n    \"productionExpediteRequestId\": {\n      \"description\": \"Uniquely identifies the expedite activation request of the configuration version on the production network.\",\n      \"type\": \"integer\"\n    },\n    \"stagingActiveVersion\": {\n      \"description\": \"The version number of the security configuration that is currently active on the staging network.\",\n      \"type\": \"integer\"\n    },\n    \"stagingExpediteRequestId\": {\n      \"description\": \"Uniquely identifies the expedite activation request of the configuration version on the staging network.\",\n      \"type\": \"integer\"\n    },\n    \"totalSize\": {\n      \"description\": \"The total number of configuration\
  \ versions.\",\n      \"type\": \"integer\"\n    },\n    \"versionList\": {\n      \"description\": \"The security configuration's versions.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"properties\": {\n          \"basedOn\": {\n            \"description\": \"The version from which you cloned this version.\",\n            \"type\": \"integer\"\n          },\n          \"createDate\": {\n            \"description\": \"The date when you created the configuration version.\",\n            \"type\": \"string\"\n          },\n          \"createdBy\": {\n            \"description\": \"The user who created the configuration version.\",\n            \"type\": \"string\"\n          },\n          \"production\": {\n            \"additionalProperties\": false,\n            \"description\": \"Contains details about the version's activation in the production network.\",\n            \"properties\": {\n              \"action\": {\n                \"description\": \"The\
  \ action taken on the configuration version, either `ACTIVATE` or `DEACTIVATE`.\",\n                \"enum\": [\n                  \"ACTIVATE\",\n                  \"DEACTIVATE\"\n                ],\n                \"type\": \"string\"\n              },\n              \"status\": {\n                \"description\": \"The activation status of the configuration version. Either `Pending`, `Active`, `Inactive`, `Deactivated`, or `Failed`.\",\n                \"enum\": [\n                  \"Pending\",\n                  \"Active\",\n                  \"Inactive\",\n                  \"Deactivated\",\n                  \"Failed\"\n                ],\n                \"type\": \"string\"\n              },\n              \"time\": {\n                \"description\": \"The activation time.\",\n                \"type\": \"string\"\n              }\n            },\n            \"required\": [\n              \"status\"\n            ],\n            \"type\": \"object\"\n          },\n          \"\
  staging\": {\n            \"additionalProperties\": false,\n            \"description\": \"Contains details about the version's activation in the staging network.\",\n            \"properties\": {\n              \"action\": {\n                \"description\": \"The action taken on the configuration version, either `ACTIVATE` or `DEACTIVATE`.\",\n                \"enum\": [\n                  \"ACTIVATE\",\n                  \"DEACTIVATE\"\n                ],\n                \"type\": \"string\"\n              },\n              \"status\": {\n                \"description\": \"The activation status of the configuration version. Either `Pending`, `Active`, `Inactive`, `Deactivated`, or `Failed`.\",\n                \"enum\": [\n                  \"Pending\",\n                  \"Active\",\n                  \"Inactive\",\n                  \"Deactivated\",\n                  \"Failed\"\n                ],\n                \"type\": \"string\"\n              },\n              \"time\": {\n\
  \                \"description\": \"The activation time.\",\n                \"type\": \"string\"\n              }\n            },\n            \"required\": [\n              \"status\"\n            ],\n            \"type\": \"object\"\n          },\n          \"version\": {\n            \"description\": \"The security configuration's version.\",\n            \"type\": \"integer\"\n          },\n          \"versionNotes\": {\n            \"description\": \"The notes you entered for the configuration version.\",\n            \"type\": \"string\"\n          }\n        },\n        \"required\": [\n          \"production\",\n          \"staging\",\n          \"version\"\n        ],\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"configId\",\n    \"configName\",\n    \"lastCreatedVersion\",\n    \"page\",\n    \"pageSize\",\n    \"totalSize\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-waf-config-versions-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: waf-config-versions
---
