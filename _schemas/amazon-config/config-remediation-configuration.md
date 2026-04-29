---
description: An object that represents the details about the remediation configuration that includes the remediation action, parameters, and data to execute the action.
layout: schema
name: RemediationConfiguration
properties_list:
- description: ''
  name: ConfigRuleName
  type: object
- description: ''
  name: TargetType
  type: object
- description: ''
  name: TargetId
  type: object
- description: ''
  name: TargetVersion
  type: object
- description: ''
  name: Parameters
  type: object
- description: ''
  name: ResourceType
  type: object
- description: ''
  name: Automatic
  type: object
- description: ''
  name: ExecutionControls
  type: object
- description: ''
  name: MaximumAutomaticAttempts
  type: object
- description: ''
  name: RetryAttemptSeconds
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: CreatedByService
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-remediation-configuration-schema.json
slug: config-remediation-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-remediation-configuration-schema.json\",\n  \"title\": \"RemediationConfiguration\",\n  \"description\": \"An object that represents the details about the remediation configuration that includes the remediation action, parameters, and data to execute the action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRuleName\"\n        },\n        {\n          \"description\": \"The name of the Config rule.\"\n        }\n      ]\n    },\n    \"TargetType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemediationTargetType\"\n        },\n        {\n          \"description\": \"The type of the target. Target executes remediation. For example, SSM document.\"\n      \
  \  }\n      ]\n    },\n    \"TargetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"Target ID is the name of the SSM document.\"\n        }\n      ]\n    },\n    \"TargetVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>Version of the target. For example, version of the SSM document.</p> <note> <p>If you make backward incompatible changes to the SSM document, you must call PutRemediationConfiguration API again to ensure the remediations can run.</p> </note>\"\n        }\n      ]\n    },\n    \"Parameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemediationParameters\"\n        },\n        {\n          \"description\": \"An object of the RemediationParameterValue.\"\n        }\n      ]\n    },\n    \"ResourceType\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The type of a resource. \"\n        }\n      ]\n    },\n    \"Automatic\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"The remediation is triggered automatically.\"\n        }\n      ]\n    },\n    \"ExecutionControls\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionControls\"\n        },\n        {\n          \"description\": \"An ExecutionControls object.\"\n        }\n      ]\n    },\n    \"MaximumAutomaticAttempts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoRemediationAttempts\"\n        },\n        {\n          \"description\": \"<p>The maximum number of failed attempts for auto-remediation. If you do not select a number, the default is 5.</p> <p>For example, if you specify MaximumAutomaticAttempts\
  \ as 5 with RetryAttemptSeconds as 50 seconds, Config will put a RemediationException on your behalf for the failing resource after the 5th failed attempt within 50 seconds.</p>\"\n        }\n      ]\n    },\n    \"RetryAttemptSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoRemediationAttemptSeconds\"\n        },\n        {\n          \"description\": \"<p>Maximum time in seconds that Config runs auto-remediation. If you do not select a number, the default is 60 seconds. </p> <p>For example, if you specify RetryAttemptSeconds as 50 seconds and MaximumAutomaticAttempts as 5, Config will run auto-remediations 5 times within 50 seconds before throwing an exception.</p>\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit1024\"\n        },\n        {\n          \"description\": \"Amazon Resource Name (ARN) of remediation configuration.\"\n        }\n      ]\n\
  \    },\n    \"CreatedByService\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit1024\"\n        },\n        {\n          \"description\": \"Name of the service that owns the service-linked rule, if applicable.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigRuleName\",\n    \"TargetType\",\n    \"TargetId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-remediation-configuration-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: RemediationConfiguration
---
