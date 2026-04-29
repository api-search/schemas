---
description: <p>Status information for your Config Managed rules and Config Custom Policy rules. The status includes information such as the last time the rule ran, the last time it failed, and the related error for the last failure.</p> <p>This action does not return status information about Config Custom Lambda rules.</p>
layout: schema
name: ConfigRuleEvaluationStatus
properties_list:
- description: ''
  name: ConfigRuleName
  type: object
- description: ''
  name: ConfigRuleArn
  type: object
- description: ''
  name: ConfigRuleId
  type: object
- description: ''
  name: LastSuccessfulInvocationTime
  type: object
- description: ''
  name: LastFailedInvocationTime
  type: object
- description: ''
  name: LastSuccessfulEvaluationTime
  type: object
- description: ''
  name: LastFailedEvaluationTime
  type: object
- description: ''
  name: FirstActivatedTime
  type: object
- description: ''
  name: LastDeactivatedTime
  type: object
- description: ''
  name: LastErrorCode
  type: object
- description: ''
  name: LastErrorMessage
  type: object
- description: ''
  name: FirstEvaluationStarted
  type: object
- description: ''
  name: LastDebugLogDeliveryStatus
  type: object
- description: ''
  name: LastDebugLogDeliveryStatusReason
  type: object
- description: ''
  name: LastDebugLogDeliveryTime
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-config-rule-evaluation-status-schema.json
slug: config-config-rule-evaluation-status
source_filename: config-config-rule-evaluation-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-config-rule-evaluation-status-schema.json\",\n  \"title\": \"ConfigRuleEvaluationStatus\",\n  \"description\": \"<p>Status information for your Config Managed rules and Config Custom Policy rules. The status includes information such as the last time the rule ran, the last time it failed, and the related error for the last failure.</p> <p>This action does not return status information about Config Custom Lambda rules.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRuleName\"\n        },\n        {\n          \"description\": \"The name of the Config rule.\"\n        }\n      ]\n    },\n    \"ConfigRuleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\
  \n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Config rule.\"\n        }\n      ]\n    },\n    \"ConfigRuleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ID of the Config rule.\"\n        }\n      ]\n    },\n    \"LastSuccessfulInvocationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time that Config last successfully invoked the Config rule to evaluate your Amazon Web Services resources.\"\n        }\n      ]\n    },\n    \"LastFailedInvocationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time that Config last failed to invoke the Config rule to evaluate your Amazon Web Services resources.\"\n        }\n      ]\n    },\n    \"LastSuccessfulEvaluationTime\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time that Config last successfully evaluated your Amazon Web Services resources against the rule.\"\n        }\n      ]\n    },\n    \"LastFailedEvaluationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time that Config last failed to evaluate your Amazon Web Services resources against the rule.\"\n        }\n      ]\n    },\n    \"FirstActivatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time that you first activated the Config rule.\"\n        }\n      ]\n    },\n    \"LastDeactivatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time that you\
  \ last turned off the Config rule.\"\n        }\n      ]\n    },\n    \"LastErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The error code that Config returned when the rule last failed.\"\n        }\n      ]\n    },\n    \"LastErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The error message that Config returned when the rule last failed.\"\n        }\n      ]\n    },\n    \"FirstEvaluationStarted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>Indicates whether Config has evaluated your resources against the rule at least once.</p> <ul> <li> <p> <code>true</code> - Config has evaluated your Amazon Web Services resources against the rule at least once.</p> </li> <li> <p> <code>false</code>\
  \ - Config has not finished evaluating your Amazon Web Services resources against the rule at least once.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"LastDebugLogDeliveryStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The status of the last attempted delivery of a debug log for your Config Custom Policy rules. Either <code>Successful</code> or <code>Failed</code>.\"\n        }\n      ]\n    },\n    \"LastDebugLogDeliveryStatusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The reason Config was not able to deliver a debug log. This is for the last failed attempt to retrieve a debug log for your Config Custom Policy rules.\"\n        }\n      ]\n    },\n    \"LastDebugLogDeliveryTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n\
  \        {\n          \"description\": \"The time Config last attempted to deliver a debug log for your Config Custom Policy rules.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-config-rule-evaluation-status-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ConfigRuleEvaluationStatus
---
