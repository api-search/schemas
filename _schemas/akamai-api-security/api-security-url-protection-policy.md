---
description: Contains details about a URL protection policy.
layout: schema
name: url-protection-policy
properties_list:
- description: The API endpoints to match on in incoming requests. This only applies to the `api` `matchType`.
  name: apiDefinitions
  type: array
- description: Exempts specific clients from being processed by the URL protection policy.
  name: bypassCondition
  type: object
- description: The traffic categories to perform load shedding on when the origin traffic rate exceeds the load shedding threshold. If `intelligentLoadShedding` is set to `true`, specify one or more categories.
  name: categories
  type: array
- description: Uniquely identifies the security configuration.
  name: configId
  type: integer
- description: The security configuration version.
  name: configVersion
  type: integer
- description: __Read-only__ The timestamp when you created the URL protection policy.
  name: createDate
  type: string
- description: __Read-only__ The username of the person who created the URL protection policy.
  name: createdBy
  type: string
- description: A description of the rate policy.
  name: description
  type: string
- description: The hostname and path combinations to match on.
  name: hostnamePaths
  type: array
- description: Enable or disable intelligent load shedding. If enabled, traffic that matches the load shedding categories is eligible for shedding if the origin rate exceeds the load shedding threshold.
  name: intelligentLoadShedding
  type: boolean
- description: The rate policy's unique name.
  name: name
  type: string
- description: __Read-only__ Uniquely identifies the URL protection policy.
  name: policyId
  type: integer
- description: If matching on `hostnamePaths`, specify `SINGLE` to match on a hostname and path, or `MULTIPLE` to match on hostname and path combinations.
  name: protectionType
  type: string
- description: The allowed hits per second during any five-second interval.
  name: rateThreshold
  type: integer
- description: Specify the threshold value, in hits per second, after which traffic can be shed. The `sheddingThresholdHitsPerSec` value must be between 70%-90% of the `rateThreshold` value. If you enabled `intellig
  name: sheddingThresholdHitsPerSec
  type: integer
- description: __Read-only__ The ISO 8601 timestamp when you last updated the URL protection policy.
  name: updateDate
  type: string
- description: __Read-only__ Username who last updated the URL protection policy.
  name: updatedBy
  type: string
- description: __Read-only__ Whether you're currently using the URL protection policy.
  name: used
  type: boolean
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-url-protection-policy-schema.json
slug: api-security-url-protection-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-url-protection-policy-schema.json\",\n  \"title\": \"url-protection-policy\",\n  \"description\": \"Contains details about a URL protection policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiDefinitions\": {\n      \"description\": \"The API endpoints to match on in incoming requests. This only applies to the `api` `matchType`.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"properties\": {\n          \"apiDefinitionId\": {\n            \"description\": \"Uniquely identifies each API endpoint.\",\n            \"format\": \"int64\",\n            \"type\": \"integer\"\n          },\n          \"definedResources\": {\n            \"description\": \"When `true`, match on any resource explicitly added to your API definition without including a `resourceId`.\
  \ When `false`, you'll need to pass a `resourceId`.\",\n            \"type\": \"boolean\"\n          },\n          \"resourceIds\": {\n            \"description\": \"The unique identifiers of the endpoint's resources.\",\n            \"items\": {\n              \"format\": \"int64\",\n              \"type\": \"integer\"\n            },\n            \"type\": \"array\"\n          },\n          \"undefinedResources\": {\n            \"description\": \"When `true`, match on any resource you have not explicitly added to your API definition without including a `resourceId`.  When `false`, you'll need to pass a `resourceId`.\",\n            \"type\": \"boolean\"\n          }\n        },\n        \"required\": [\n          \"apiDefinitionId\"\n        ],\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    },\n    \"bypassCondition\": {\n      \"additionalProperties\": false,\n      \"description\": \"Exempts specific clients from being processed by the URL protection policy.\"\
  ,\n      \"properties\": {\n        \"atomicConditions\": {\n          \"description\": \"Specify one or more types of conditions to match on. You can match on client lists, request headers, or both.\",\n          \"items\": {\n            \"oneOf\": [\n              {\n                \"additionalProperties\": false,\n                \"description\": \"Collects data needed for condition matches on request headers.\",\n                \"properties\": {\n                  \"className\": {\n                    \"description\": \"Choose `RequestHeaderCondition` to match a header from the requesting client to the specified header.\",\n                    \"enum\": [\n                      \"RequestHeaderCondition\"\n                    ],\n                    \"type\": \"string\"\n                  },\n                  \"name\": {\n                    \"description\": \"Use `name` to check whether the specified header exists.\",\n                    \"items\": {\n                      \"\
  minLength\": 1,\n                      \"type\": \"string\"\n                    },\n                    \"minItems\": 1,\n                    \"type\": \"array\",\n                    \"uniqueItems\": true\n                  },\n                  \"nameWildcard\": {\n                    \"description\": \"Whether to interpret `?` and `*` as wildcards in the specified `name`.\",\n                    \"type\": \"boolean\"\n                  },\n                  \"positiveMatch\": {\n                    \"description\": \"__Read-only__ Whether the condition triggers on a match or lack of match.\",\n                    \"readOnly\": true,\n                    \"type\": \"boolean\"\n                  },\n                  \"value\": {\n                    \"description\": \"A list of unique header values. Use both `value` and `name` to check whether the requesting client\\u2019s header matches the specified headers.\",\n                    \"items\": {\n                      \"minLength\"\
  : 1,\n                      \"type\": \"string\"\n                    },\n                    \"nullable\": true,\n                    \"type\": \"array\",\n                    \"uniqueItems\": true\n                  },\n                  \"valueCase\": {\n                    \"description\": \"Whether to consider case when matching header values, `true` for case-sensitive matches.\",\n                    \"type\": \"boolean\"\n                  },\n                  \"valueWildcard\": {\n                    \"description\": \"Whether to interpret `?` and `*` as wildcards in the specified `value`.\",\n                    \"type\": \"boolean\"\n                  }\n                },\n                \"required\": [\n                  \"className\",\n                  \"name\"\n                ],\n                \"title\": \"RequestHeaderCondition\",\n                \"type\": \"object\",\n                \"x-akamai\": {\n                  \"file-path\": \"schemas/url-protection-bypass-request-header-condition.yaml\"\
  \n                }\n              },\n              {\n                \"additionalProperties\": false,\n                \"description\": \"Collects data needed for condition matches on client lists and network lists.\",\n                \"properties\": {\n                  \"checkIps\": {\n                    \"description\": \"__Read-only__ Whether the connecting IP or both the connecting IP and `X-Forwarded-For` (XFF) header match on the client list or network list. URL protection bypass supports `connecting` only.\",\n                    \"enum\": [\n                      \"connecting\"\n                    ],\n                    \"readOnly\": true,\n                    \"type\": \"string\"\n                  },\n                  \"className\": {\n                    \"description\": \"Choose `NetworkListCondition` to match the requesting client's identifier, like IP, GEO, ASN or TLS Fingerprint, against the specified client list or network list.\",\n                    \"enum\"\
  : [\n                      \"NetworkListCondition\"\n                    ],\n                    \"type\": \"string\"\n                  },\n                  \"positiveMatch\": {\n                    \"description\": \"__Read-only__ Whether the condition triggers on a match or lack of match.\",\n                    \"readOnly\": true,\n                    \"type\": \"boolean\"\n                  },\n                  \"value\": {\n                    \"description\": \"Identifies the client list or network list.\",\n                    \"items\": {\n                      \"minLength\": 1,\n                      \"type\": \"string\"\n                    },\n                    \"nullable\": true,\n                    \"type\": \"array\",\n                    \"uniqueItems\": true\n                  }\n                },\n                \"required\": [\n                  \"className\",\n                  \"value\"\n                ],\n                \"title\": \"NetworkListCondition\"\
  ,\n                \"type\": \"object\",\n                \"x-akamai\": {\n                  \"file-path\": \"schemas/url-protection-bypass-client-list-condition.yaml\"\n                }\n              }\n            ]\n          },\n          \"minItems\": 1,\n          \"type\": \"array\"\n        }\n      },\n      \"type\": \"object\"\n    },\n    \"categories\": {\n      \"description\": \"The traffic categories to perform load shedding on when the origin traffic rate exceeds the load shedding threshold. If `intelligentLoadShedding` is set to `true`, specify one or more categories.\",\n      \"items\": {\n        \"oneOf\": [\n          {\n            \"additionalProperties\": false,\n            \"description\": \"Specify one or more load shedding categories for the URL protection policy.\",\n            \"properties\": {\n              \"type\": {\n                \"description\": \"Specify the type of traffic to shed first before reaching the requests per second (RPS) limit. `BOTS`\
  \ includes bots from Akamai's existing list of known bots. `CLIENT_REPUTATIONS` includes traffic from clients with a bad client reputation score. `CLOUD_PROVIDERS` includes traffic from providers like AWS, Microsoft Azure, and Google Cloud. `PROXIES` includes proxy traffic as determined by IPQualityScore (IPQS) and Akamai EdgeScape. `TOR_EXIT_NODES` includes traffic defined in Akamai's existing network list of nodes. `PLATFORM_DDOS_INTELLIGENCE` includes traffic detected by Akamai's DDOS Intelligence platform.\",\n                \"enum\": [\n                  \"BOTS\",\n                  \"CLIENT_REPUTATIONS\",\n                  \"CLOUD_PROVIDERS\",\n                  \"PROXIES\",\n                  \"TOR_EXIT_NODES\",\n                  \"PLATFORM_DDOS_INTELLIGENCE\"\n                ],\n                \"type\": \"string\"\n              }\n            },\n            \"required\": [\n              \"type\"\n            ],\n            \"title\": \"Client list category\",\n       \
  \     \"type\": \"object\",\n            \"x-akamai\": {\n              \"file-path\": \"schemas/url-protection-category.yaml\"\n            }\n          },\n          {\n            \"additionalProperties\": false,\n            \"description\": \"Defines a `CLIENT_LIST` load shedding category for a URL protection policy.\",\n            \"properties\": {\n              \"listIds\": {\n                \"description\": \"A list of client list identifiers to match on.\",\n                \"items\": {\n                  \"type\": \"string\"\n                },\n                \"type\": \"array\"\n              },\n              \"positiveMatch\": {\n                \"description\": \"Whether the selected client lists match.\",\n                \"type\": \"boolean\"\n              },\n              \"type\": {\n                \"description\": \"Specify `CLIENT_LIST` to match on a client list.\",\n                \"enum\": [\n                  \"CLIENT_LIST\"\n                ],\n       \
  \         \"type\": \"string\"\n              }\n            },\n            \"required\": [\n              \"type\"\n            ],\n            \"title\": \"Other categories\",\n            \"type\": \"object\",\n            \"x-akamai\": {\n              \"file-path\": \"schemas/url-protection-client-list-category.yaml\"\n            }\n          }\n        ]\n      },\n      \"type\": \"array\"\n    },\n    \"configId\": {\n      \"description\": \"Uniquely identifies the security configuration.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"configVersion\": {\n      \"description\": \"The security configuration version.\",\n      \"type\": \"integer\"\n    },\n    \"createDate\": {\n      \"description\": \"__Read-only__ The timestamp when you created the URL protection policy.\",\n      \"format\": \"date-time\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"createdBy\": {\n      \"description\": \"__Read-only__ The username of\
  \ the person who created the URL protection policy.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"A description of the rate policy.\",\n      \"type\": \"string\"\n    },\n    \"hostnamePaths\": {\n      \"description\": \"The hostname and path combinations to match on.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"description\": \"The hostname and path combinations to match on.\",\n        \"properties\": {\n          \"hostname\": {\n            \"description\": \"The hostnames you choose to match on.\",\n            \"type\": \"string\"\n          },\n          \"paths\": {\n            \"description\": \"The list of paths to match on.\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"type\": \"array\"\n          }\n        },\n        \"required\": [\n          \"hostname\",\n          \"paths\"\n        ],\n        \"type\": \"object\",\n\
  \        \"x-akamai\": {\n          \"file-path\": \"schemas/url-protection-policy-hostpath.yaml\"\n        }\n      },\n      \"minItems\": 1,\n      \"type\": \"array\"\n    },\n    \"intelligentLoadShedding\": {\n      \"description\": \"Enable or disable intelligent load shedding. If enabled, traffic that matches the load shedding categories is eligible for shedding if the origin rate exceeds the load shedding threshold.\",\n      \"type\": \"boolean\"\n    },\n    \"name\": {\n      \"description\": \"The rate policy's unique name.\",\n      \"type\": \"string\"\n    },\n    \"policyId\": {\n      \"description\": \"__Read-only__ Uniquely identifies the URL protection policy.\",\n      \"format\": \"int64\",\n      \"readOnly\": true,\n      \"type\": \"integer\"\n    },\n    \"protectionType\": {\n      \"description\": \"If matching on `hostnamePaths`, specify `SINGLE` to match on a hostname and path, or `MULTIPLE` to match on hostname and path combinations.\",\n      \"enum\":\
  \ [\n        \"SINGLE\",\n        \"MULTIPLE\"\n      ],\n      \"type\": \"string\"\n    },\n    \"rateThreshold\": {\n      \"description\": \"The allowed hits per second during any five-second interval.\",\n      \"type\": \"integer\"\n    },\n    \"sheddingThresholdHitsPerSec\": {\n      \"description\": \"Specify the threshold value, in hits per second, after which traffic can be shed. The `sheddingThresholdHitsPerSec` value must be between 70%-90% of the `rateThreshold` value. If you enabled `intelligentLoadShedding`, this value is required.\",\n      \"type\": \"integer\"\n    },\n    \"updateDate\": {\n      \"description\": \"__Read-only__ The ISO 8601 timestamp when you last updated the URL protection policy.\",\n      \"format\": \"date-time\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"updatedBy\": {\n      \"description\": \"__Read-only__ Username who last updated the URL protection policy.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\
  \n    },\n    \"used\": {\n      \"description\": \"__Read-only__ Whether you're currently using the URL protection policy.\",\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"intelligentLoadShedding\",\n    \"rateThreshold\",\n    \"name\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-url-protection-policy-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: url-protection-policy
---
