---
description: Contains settings for a custom rule.
layout: schema
name: custom-rule
properties_list:
- description: Contains the details about the condition that triggers the custom rule.
  name: conditions
  type: array
- description: The custom rule description.
  name: description
  type: string
- description: The time period during which the custom rule is active.
  name: effectiveTimePeriod
  type: object
- description: Uniquely identifies the rule.
  name: id
  type: integer
- description: Whether to inspect the HTTP request for unstructured custom rules.
  name: inspectRequest
  type: boolean
- description: Whether to inspect the HTTP response for unstructured custom rules.
  name: inspectResponse
  type: boolean
- description: The specific conditions to be logged.
  name: loggingOptions
  type: array
- description: The metadata you provided for unstructured custom rules.
  name: metadata
  type: string
- description: The custom rule name.
  name: name
  type: string
- description: Specify `AND` logic to require all conditions, or `OR` logic to require at least one condition to match.
  name: operation
  type: string
- description: Whether the rule is active in the configuration.
  name: ruleActivated
  type: boolean
- description: The portion of traffic to sample, expressed as a percent.
  name: samplingRate
  type: integer
- description: Whether to show traffic from only the staging network, or all traffic. The default setting is `false` and only shows in the response when `true`.
  name: stagingOnly
  type: boolean
- description: Whether you created the rule with the structured custom rule builder or free-form XML. This needs to be `true`.
  name: structured
  type: boolean
- description: The list of labels you assigned to the custom rule.
  name: tag
  type: array
- description: The custom rule version.
  name: version
  type: integer
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-custom-rule-schema.json
slug: api-security-custom-rule
source_filename: api-security-custom-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-custom-rule-schema.json\",\n  \"title\": \"custom-rule\",\n  \"description\": \"Contains settings for a custom rule.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"conditions\": {\n      \"description\": \"Contains the details about the condition that triggers the custom rule.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"properties\": {\n          \"name\": {\n            \"description\": \"The name you assign to the custom rule.\",\n            \"oneOf\": [\n              {\n                \"items\": {\n                  \"type\": \"string\"\n                },\n                \"title\": \"Array\",\n                \"type\": \"array\"\n              },\n              {\n                \"title\": \"String\",\n                \"type\": \"string\"\
  \n              }\n            ]\n          },\n          \"nameCase\": {\n            \"description\": \"Whether to consider the case-sensitivity of the provided query parameter `name`. This only applies to the `uriQueryMatch` condition `type`.\",\n            \"type\": \"boolean\"\n          },\n          \"nameWildcard\": {\n            \"description\": \"Whether the provided header `name` is a wildcard. This only applies to the `requestHeaderMatch` condition `type`.\",\n            \"type\": \"boolean\"\n          },\n          \"positiveMatch\": {\n            \"description\": \"Whether the condition should trigger on a match (`true`) or a lack of match (`false`).\",\n            \"type\": \"boolean\"\n          },\n          \"type\": {\n            \"description\": \"The type of condition. See [CustomRule condition type values](https://techdocs.akamai.com/application-security/reference/condition-type-values).\",\n            \"enum\": [\n              \"cookieMatch\",\n        \
  \      \"extensionMatch\",\n              \"filenameMatch\",\n              \"ipMatch\",\n              \"pathMatch\",\n              \"requestHeaderMatch\",\n              \"requestMethodMatch\",\n              \"requestProtocolVersionMatch\",\n              \"uriQueryMatch\",\n              \"headerOrderMatch\",\n              \"argsPostMatch\",\n              \"argsPostNamesMatch\",\n              \"clientCertPresentMatch\",\n              \"clientCertValidMatch\",\n              \"clientTlsFingerprintMatch\",\n              \"hostMatch\",\n              \"ipAddressMatch\",\n              \"geoMatch\",\n              \"asNumberMatch\",\n              \"clientListMatch\"\n            ],\n            \"type\": \"string\"\n          },\n          \"useXForwardForHeaders\": {\n            \"description\": \"Whether the condition should include `X-Forwarded-For` (XFF) header. This only applies when the `type` is `ipAddressMatch`, `geoMatch`, `asNumberMatch`, or `clientListMatch`.\",\n  \
  \          \"type\": \"boolean\"\n          },\n          \"value\": {\n            \"description\": \"The value that triggers the condition when matched or not matched. Specify a string for the `requestProtocolVersionMatch`, `clientCertPresentMatch`, `clientCertValidMatch`, and `headerOrderMatch` conditions. For all other conditions, specify an array of strings.\",\n            \"oneOf\": [\n              {\n                \"items\": {\n                  \"type\": \"string\"\n                },\n                \"title\": \"Array\",\n                \"type\": \"array\"\n              },\n              {\n                \"title\": \"String\",\n                \"type\": \"string\"\n              }\n            ],\n            \"type\": \"string\"\n          },\n          \"valueCase\": {\n            \"description\": \"Whether to consider the case-sensitivity of the provided header `value`. This only applies to the `requestHeaderMatch` condition `type`.\",\n            \"type\": \"boolean\"\
  \n          },\n          \"valueExactMatch\": {\n            \"description\": \"Whether to consider only exact matches of the header `value`.\",\n            \"type\": \"boolean\"\n          },\n          \"valueIgnoreSegment\": {\n            \"description\": \"Whether to ignore path segments when matching. This only applies when the `type` is `pathMatch`.\",\n            \"type\": \"boolean\"\n          },\n          \"valueNormalize\": {\n            \"description\": \"Whether to normalize the value of the header when matching. This only applies to type values of `extensionMatch` and `pathMatch`.\",\n            \"type\": \"boolean\"\n          },\n          \"valueRecursive\": {\n            \"description\": \"Whether to use recursion when matching. When `false`, you can only match on the filename in the root folder. This only applies when the condition `type` is `filenameMatch`.\",\n            \"type\": \"boolean\"\n          },\n          \"valueWildcard\": {\n            \"description\"\
  : \"Whether the provided header `value` is a wildcard. This only applies when the condition `type` is `requestHeaderMatch`.\",\n            \"type\": \"boolean\"\n          }\n        },\n        \"required\": [\n          \"type\",\n          \"positiveMatch\"\n        ],\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    },\n    \"description\": {\n      \"description\": \"The custom rule description.\",\n      \"type\": \"string\"\n    },\n    \"effectiveTimePeriod\": {\n      \"additionalProperties\": false,\n      \"description\": \"The time period during which the custom rule is active.\",\n      \"properties\": {\n        \"endDate\": {\n          \"description\": \"An ISO 8601 timestamp that sets when the rule expires or deactivates.\",\n          \"type\": \"string\"\n        },\n        \"startDate\": {\n          \"description\": \"An ISO 8601 timestamp that sets when the rule activates.\",\n          \"format\": \"date-time\",\n          \"type\": \"string\"\
  \n        },\n        \"status\": {\n          \"description\": \"The current status of the rule based on its `startDate` and `endDate`. By default, rules are active for 30 days. When `ACTIVE`, the rule triggers when conditions are met. When `INACTIVE`, the rule doesn't trigger. When `EXPIRING`, the rule still triggers because it's still active until its specified expiration date. When the rule's status is `EXPIRED`, the rule is inactive and doesn't trigger. If your rule expires and you want to use it again, make a PUT request to [Modify a custom rule](https://techdocs.akamai.com/application-security/reference/put-config-custom-rule) with the new dates you'd like the rule to be active.\",\n          \"enum\": [\n            \"active\",\n            \"inactive\",\n            \"expiring\",\n            \"expired\"\n          ],\n          \"type\": \"string\"\n        }\n      },\n      \"required\": [\n        \"endDate\",\n        \"startDate\"\n      ],\n      \"type\": \"object\"\n\
  \    },\n    \"id\": {\n      \"description\": \"Uniquely identifies the rule.\",\n      \"type\": \"integer\"\n    },\n    \"inspectRequest\": {\n      \"description\": \"Whether to inspect the HTTP request for unstructured custom rules.\",\n      \"type\": \"boolean\"\n    },\n    \"inspectResponse\": {\n      \"description\": \"Whether to inspect the HTTP response for unstructured custom rules.\",\n      \"type\": \"boolean\"\n    },\n    \"loggingOptions\": {\n      \"description\": \"The specific conditions to be logged.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"description\": \"Condition to be logged.\",\n        \"properties\": {\n          \"id\": {\n            \"description\": \"The unique identifier for each logging option. See [Logging option values](https://techdocs.akamai.com/application-security/reference/logging-option-values).\",\n            \"enum\": [\n              \"CLIENT_TLS_FINGERPRINT_MATCH\",\n              \"HEADER_ORDER_MATCH\"\
  ,\n              \"REQUEST_HEADER_MATCH\",\n              \"COOKIE_MATCH\",\n              \"URI_QUERY_MATCH\",\n              \"ARGS_POST_MATCH\"\n            ],\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"description\": \"A description of the logging option type.\",\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"description\": \"The value on which to match when determining whether to log the custom rule condition.\",\n            \"type\": \"string\"\n          }\n        },\n        \"required\": [\n          \"id\"\n        ],\n        \"type\": \"object\",\n        \"x-akamai\": {\n          \"file-path\": \"schemas/logging-option.yaml\"\n        }\n      },\n      \"type\": \"array\"\n    },\n    \"metadata\": {\n      \"description\": \"The metadata you provided for unstructured custom rules.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The custom rule name.\",\n\
  \      \"type\": \"string\"\n    },\n    \"operation\": {\n      \"description\": \"Specify `AND` logic to require all conditions, or `OR` logic to require at least one condition to match.\",\n      \"enum\": [\n        \"AND\",\n        \"OR\"\n      ],\n      \"type\": \"string\"\n    },\n    \"ruleActivated\": {\n      \"description\": \"Whether the rule is active in the configuration.\",\n      \"type\": \"boolean\"\n    },\n    \"samplingRate\": {\n      \"description\": \"The portion of traffic to sample, expressed as a percent.\",\n      \"maximum\": 100,\n      \"minimum\": 0,\n      \"type\": \"integer\"\n    },\n    \"stagingOnly\": {\n      \"default\": false,\n      \"description\": \"Whether to show traffic from only the staging network, or all traffic. The default setting is `false` and only shows in the response when `true`. \",\n      \"type\": \"boolean\"\n    },\n    \"structured\": {\n      \"description\": \"Whether you created the rule with the structured custom rule\
  \ builder or free-form XML. This needs to be `true`.\",\n      \"type\": \"boolean\"\n    },\n    \"tag\": {\n      \"description\": \"The list of labels you assigned to the custom rule.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"version\": {\n      \"description\": \"The custom rule version.\",\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"operation\",\n    \"structured\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-custom-rule-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: custom-rule
---
