---
description: <p>The proposed access control configuration for an Amazon ECR repository. You can propose a configuration for a new Amazon ECR repository or an existing Amazon ECR repository that you own by specifying the Amazon ECR policy. For more information, see <a href="https://docs.aws.amazon.com/AmazonECR/latest/APIReference/API_Repository.html">Repository</a>.</p> <ul> <li> <p>If the configuration is for an existing Amazon ECR repository and you do not specify the Amazon ECR policy, then the access preview uses the existing Amazon ECR policy for the repository.</p> </li> <li> <p>If the access preview is for a new resource and you do not specify the policy, then the access preview assumes an Amazon ECR repository without a policy.</p> </li> <li> <p>To propose deletion of an existing Amazon ECR repository policy, you can specify an empty string for the Amazon ECR policy.</p> </li> </ul>
layout: schema
name: EcrRepositoryConfiguration
properties_list:
- description: ''
  name: repositoryPolicy
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-ecr-repository-configuration-schema.json
slug: iam-access-analyzer-ecr-repository-configuration
source_filename: iam-access-analyzer-ecr-repository-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-ecr-repository-configuration-schema.json\",\n  \"title\": \"EcrRepositoryConfiguration\",\n  \"description\": \"<p>The proposed access control configuration for an Amazon ECR repository. You can propose a configuration for a new Amazon ECR repository or an existing Amazon ECR repository that you own by specifying the Amazon ECR policy. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonECR/latest/APIReference/API_Repository.html\\\">Repository</a>.</p> <ul> <li> <p>If the configuration is for an existing Amazon ECR repository and you do not specify the Amazon ECR policy, then the access preview uses the existing Amazon ECR policy for the repository.</p> </li> <li> <p>If the access preview is for a new resource and you do not specify the policy, then the\
  \ access preview assumes an Amazon ECR repository without a policy.</p> </li> <li> <p>To propose deletion of an existing Amazon ECR repository policy, you can specify an empty string for the Amazon ECR policy.</p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repositoryPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EcrRepositoryPolicy\"\n        },\n        {\n          \"description\": \"The JSON repository policy text to apply to the Amazon ECR repository. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonECR/latest/userguide/repository-policy-examples.html\\\">Private repository policy examples</a> in the <i>Amazon ECR User Guide</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-ecr-repository-configuration-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: EcrRepositoryConfiguration
---
