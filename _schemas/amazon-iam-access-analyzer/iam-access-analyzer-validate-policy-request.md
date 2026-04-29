---
description: ValidatePolicyRequest schema from AWS IAM Access Analyzer API
layout: schema
name: ValidatePolicyRequest
properties_list:
- description: ''
  name: locale
  type: object
- description: ''
  name: policyDocument
  type: object
- description: ''
  name: policyType
  type: object
- description: ''
  name: validatePolicyResourceType
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-validate-policy-request-schema.json
slug: iam-access-analyzer-validate-policy-request
source_filename: iam-access-analyzer-validate-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-validate-policy-request-schema.json\",\n  \"title\": \"ValidatePolicyRequest\",\n  \"description\": \"ValidatePolicyRequest schema from AWS IAM Access Analyzer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"locale\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Locale\"\n        },\n        {\n          \"description\": \"The locale to use for localizing the findings.\"\n        }\n      ]\n    },\n    \"policyDocument\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyDocument\"\n        },\n        {\n          \"description\": \"The JSON policy document to use as the content for the policy.\"\n        }\n      ]\n    },\n    \"policyType\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/PolicyType\"\n        },\n        {\n          \"description\": \"<p>The type of policy to validate. Identity policies grant permissions to IAM principals. Identity policies include managed and inline policies for IAM roles, users, and groups. They also include service-control policies (SCPs) that are attached to an Amazon Web Services organization, organizational unit (OU), or an account.</p> <p>Resource policies grant permissions on Amazon Web Services resources. Resource policies include trust policies for IAM roles and bucket policies for Amazon S3 buckets. You can provide a generic input such as identity policy or resource policy or a specific input such as managed policy or Amazon S3 bucket policy. </p>\"\n        }\n      ]\n    },\n    \"validatePolicyResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValidatePolicyResourceType\"\n        },\n        {\n          \"description\": \"<p>The type of resource to attach\
  \ to your resource policy. Specify a value for the policy validation resource type only if the policy type is <code>RESOURCE_POLICY</code>. For example, to validate a resource policy to attach to an Amazon S3 bucket, you can choose <code>AWS::S3::Bucket</code> for the policy validation resource type.</p> <p>For resource types not supported as valid values, IAM Access Analyzer runs policy checks that apply to all resource policies. For example, to validate a resource policy to attach to a KMS key, do not specify a value for the policy validation resource type and IAM Access Analyzer will run policy checks that apply to all resource policies.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"policyDocument\",\n    \"policyType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-validate-policy-request-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: ValidatePolicyRequest
---
