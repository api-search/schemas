---
description: An AWS Firewall Manager policy defining security rules and resource scope.
layout: schema
name: Policy
properties_list:
- description: Unique policy identifier.
  name: PolicyId
  type: string
- description: Friendly name of the policy.
  name: PolicyName
  type: string
- description: Token for optimistic locking.
  name: PolicyUpdateToken
  type: string
- description: Details about the security service type and configuration.
  name: SecurityServicePolicyData
  type: object
- description: AWS resource type in scope.
  name: ResourceType
  type: string
- description: If True, resources with specified tags are excluded.
  name: ExcludeResourceTags
  type: boolean
- description: If True, Firewall Manager auto-remediates non-compliant resources.
  name: RemediationEnabled
  type: boolean
- description: ARN of the policy.
  name: PolicyArn
  type: string
provider_name: Amazon Firewall Manager
provider_slug: amazon-firewall-manager
schema_file: json-schema/amazon-firewall-manager-policy-schema.json
slug: amazon-firewall-manager-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-firewall-manager/refs/heads/main/json-schema/amazon-firewall-manager-policy-schema.json\",\n  \"title\": \"Policy\",\n  \"description\": \"An AWS Firewall Manager policy defining security rules and resource scope.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PolicyId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique policy identifier.\"\n    },\n    \"PolicyName\": {\n      \"type\": \"string\",\n      \"description\": \"Friendly name of the policy.\"\n    },\n    \"PolicyUpdateToken\": {\n      \"type\": \"string\",\n      \"description\": \"Token for optimistic locking.\"\n    },\n    \"SecurityServicePolicyData\": {\n      \"type\": \"object\",\n      \"description\": \"Details about the security service type and configuration.\"\n    },\n    \"ResourceType\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"AWS resource type in scope.\"\n    },\n    \"ExcludeResourceTags\": {\n      \"type\": \"boolean\",\n      \"description\": \"If True, resources with specified tags are excluded.\"\n    },\n    \"RemediationEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"If True, Firewall Manager auto-remediates non-compliant resources.\"\n    },\n    \"PolicyArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the policy.\"\n    }\n  },\n  \"required\": [\n    \"PolicyName\",\n    \"SecurityServicePolicyData\",\n    \"ResourceType\",\n    \"ExcludeResourceTags\",\n    \"RemediationEnabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-firewall-manager/refs/heads/main/json-schema/amazon-firewall-manager-policy-schema.json
tags:
- AWS
- Compliance
- Firewall
- Network Security
- Security
title: Policy
---
