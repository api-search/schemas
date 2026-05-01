---
description: Schema for an AWS Config rule resource, representing a compliance rule that evaluates whether AWS resources conform to desired configurations.
layout: schema
name: AWS Config Rule
properties_list:
- description: The name that you assign to the AWS Config rule.
  name: ConfigRuleName
  type: string
- description: The ARN of the AWS Config rule.
  name: ConfigRuleArn
  type: string
- description: The ID of the AWS Config rule.
  name: ConfigRuleId
  type: string
- description: The description that you provide for the AWS Config rule.
  name: Description
  type: string
- description: Defines which resources trigger an evaluation for the rule.
  name: Scope
  type: object
- description: Provides the rule owner, rule identifier, and notifications that cause the function to evaluate your AWS resources.
  name: Source
  type: object
- description: A string, in JSON format, that is passed to the AWS Config rule Lambda function.
  name: InputParameters
  type: string
- description: The maximum frequency with which AWS Config runs evaluations for a rule.
  name: MaximumExecutionFrequency
  type: string
- description: Indicates whether the AWS Config rule is active or is currently being deleted.
  name: ConfigRuleState
  type: string
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/amazon-config-rule-schema.json
slug: amazon-config-rule
source_filename: amazon-config-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://example.com/schemas/amazon-config-rule.json\",\n  \"title\": \"AWS Config Rule\",\n  \"description\": \"Schema for an AWS Config rule resource, representing a compliance rule that evaluates whether AWS resources conform to desired configurations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRuleName\": {\n      \"type\": \"string\",\n      \"description\": \"The name that you assign to the AWS Config rule.\",\n      \"minLength\": 1,\n      \"maxLength\": 128,\n      \"pattern\": \"^[a-zA-Z0-9-_]+$\"\n    },\n    \"ConfigRuleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the AWS Config rule.\",\n      \"pattern\": \"^arn:aws:config:[a-z0-9-]+:[0-9]{12}:config-rule/.+\"\n    },\n    \"ConfigRuleId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the AWS Config rule.\"\n    },\n    \"Description\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The description that you provide for the AWS Config rule.\",\n      \"maxLength\": 256\n    },\n    \"Scope\": {\n      \"type\": \"object\",\n      \"description\": \"Defines which resources trigger an evaluation for the rule.\",\n      \"properties\": {\n        \"ComplianceResourceTypes\": {\n          \"type\": \"array\",\n          \"description\": \"The resource types of only those AWS resources that you want to trigger an evaluation.\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"maxItems\": 100\n        },\n        \"TagKey\": {\n          \"type\": \"string\",\n          \"description\": \"The tag key that is applied to only those AWS resources that you want to trigger an evaluation.\",\n          \"maxLength\": 128\n        },\n        \"TagValue\": {\n          \"type\": \"string\",\n          \"description\": \"The tag value applied to only those AWS resources that you want to trigger an evaluation.\",\n \
  \         \"maxLength\": 256\n        },\n        \"ComplianceResourceId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the only AWS resource that you want to trigger an evaluation.\",\n          \"maxLength\": 256\n        }\n      }\n    },\n    \"Source\": {\n      \"type\": \"object\",\n      \"description\": \"Provides the rule owner, rule identifier, and notifications that cause the function to evaluate your AWS resources.\",\n      \"required\": [\"Owner\", \"SourceIdentifier\"],\n      \"properties\": {\n        \"Owner\": {\n          \"type\": \"string\",\n          \"description\": \"Indicates whether AWS or the customer owns and manages the AWS Config rule.\",\n          \"enum\": [\"CUSTOM_LAMBDA\", \"AWS\", \"CUSTOM_POLICY\"]\n        },\n        \"SourceIdentifier\": {\n          \"type\": \"string\",\n          \"description\": \"For AWS managed rules, a predefined identifier. For custom rules, the ARN of the Lambda function.\"\n        },\n\
  \        \"SourceDetails\": {\n          \"type\": \"array\",\n          \"description\": \"Provides the source and type of the event that causes AWS Config to evaluate your resources.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"EventSource\": {\n                \"type\": \"string\",\n                \"enum\": [\"aws.config\"]\n              },\n              \"MessageType\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"ConfigurationItemChangeNotification\",\n                  \"ConfigurationSnapshotDeliveryCompleted\",\n                  \"ScheduledNotification\",\n                  \"OversizedConfigurationItemChangeNotification\"\n                ]\n              },\n              \"MaximumExecutionFrequency\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"One_Hour\",\n                  \"Three_Hours\",\n                  \"Six_Hours\"\
  ,\n                  \"Twelve_Hours\",\n                  \"TwentyFour_Hours\"\n                ]\n              }\n            }\n          }\n        }\n      }\n    },\n    \"InputParameters\": {\n      \"type\": \"string\",\n      \"description\": \"A string, in JSON format, that is passed to the AWS Config rule Lambda function.\",\n      \"maxLength\": 1024\n    },\n    \"MaximumExecutionFrequency\": {\n      \"type\": \"string\",\n      \"description\": \"The maximum frequency with which AWS Config runs evaluations for a rule.\",\n      \"enum\": [\n        \"One_Hour\",\n        \"Three_Hours\",\n        \"Six_Hours\",\n        \"Twelve_Hours\",\n        \"TwentyFour_Hours\"\n      ]\n    },\n    \"ConfigRuleState\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates whether the AWS Config rule is active or is currently being deleted.\",\n      \"enum\": [\"ACTIVE\", \"DELETING\", \"DELETING_RESULTS\", \"EVALUATING\"]\n    }\n  },\n  \"required\": [\"ConfigRuleName\"\
  , \"Source\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/amazon-config-rule-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: AWS Config Rule
---
