---
description: The proposed access control configuration for an Amazon SQS queue. You can propose a configuration for a new Amazon SQS queue or an existing Amazon SQS queue that you own by specifying the Amazon SQS policy. If the configuration is for an existing Amazon SQS queue and you do not specify the Amazon SQS policy, the access preview uses the existing Amazon SQS policy for the queue. If the access preview is for a new resource and you do not specify the policy, the access preview assumes an Amazon SQS queue without a policy. To propose deletion of an existing Amazon SQS queue policy, you can specify an empty string for the Amazon SQS policy. For more information about Amazon SQS policy limits, see <a href="https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/quotas-policies.html">Quotas related to policies</a>.
layout: schema
name: SqsQueueConfiguration
properties_list:
- description: ''
  name: queuePolicy
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-sqs-queue-configuration-schema.json
slug: iam-access-analyzer-sqs-queue-configuration
source_filename: iam-access-analyzer-sqs-queue-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-sqs-queue-configuration-schema.json\",\n  \"title\": \"SqsQueueConfiguration\",\n  \"description\": \"The proposed access control configuration for an Amazon SQS queue. You can propose a configuration for a new Amazon SQS queue or an existing Amazon SQS queue that you own by specifying the Amazon SQS policy. If the configuration is for an existing Amazon SQS queue and you do not specify the Amazon SQS policy, the access preview uses the existing Amazon SQS policy for the queue. If the access preview is for a new resource and you do not specify the policy, the access preview assumes an Amazon SQS queue without a policy. To propose deletion of an existing Amazon SQS queue policy, you can specify an empty string for the Amazon SQS policy. For more information about Amazon SQS\
  \ policy limits, see <a href=\\\"https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/quotas-policies.html\\\">Quotas related to policies</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"queuePolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SqsQueuePolicy\"\n        },\n        {\n          \"description\": \" The proposed resource policy for the Amazon SQS queue. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-sqs-queue-configuration-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: SqsQueueConfiguration
---
