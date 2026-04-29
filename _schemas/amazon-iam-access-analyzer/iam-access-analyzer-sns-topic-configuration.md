---
description: The proposed access control configuration for an Amazon SNS topic. You can propose a configuration for a new Amazon SNS topic or an existing Amazon SNS topic that you own by specifying the policy. If the configuration is for an existing Amazon SNS topic and you do not specify the Amazon SNS policy, then the access preview uses the existing Amazon SNS policy for the topic. If the access preview is for a new resource and you do not specify the policy, then the access preview assumes an Amazon SNS topic without a policy. To propose deletion of an existing Amazon SNS topic policy, you can specify an empty string for the Amazon SNS policy. For more information, see <a href="https://docs.aws.amazon.com/sns/latest/api/API_Topic.html">Topic</a>.
layout: schema
name: SnsTopicConfiguration
properties_list:
- description: ''
  name: topicPolicy
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-sns-topic-configuration-schema.json
slug: iam-access-analyzer-sns-topic-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-sns-topic-configuration-schema.json\",\n  \"title\": \"SnsTopicConfiguration\",\n  \"description\": \"The proposed access control configuration for an Amazon SNS topic. You can propose a configuration for a new Amazon SNS topic or an existing Amazon SNS topic that you own by specifying the policy. If the configuration is for an existing Amazon SNS topic and you do not specify the Amazon SNS policy, then the access preview uses the existing Amazon SNS policy for the topic. If the access preview is for a new resource and you do not specify the policy, then the access preview assumes an Amazon SNS topic without a policy. To propose deletion of an existing Amazon SNS topic policy, you can specify an empty string for the Amazon SNS policy. For more information, see <a href=\\\"\
  https://docs.aws.amazon.com/sns/latest/api/API_Topic.html\\\">Topic</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"topicPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnsTopicPolicy\"\n        },\n        {\n          \"description\": \"The JSON policy text that defines who can access an Amazon SNS topic. For more information, see <a href=\\\"https://docs.aws.amazon.com/sns/latest/dg/sns-access-policy-use-cases.html\\\">Example cases for Amazon SNS access control</a> in the <i>Amazon SNS Developer Guide</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-sns-topic-configuration-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: SnsTopicConfiguration
---
