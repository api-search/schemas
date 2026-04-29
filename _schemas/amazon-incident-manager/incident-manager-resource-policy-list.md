---
description: ResourcePolicyList schema
layout: schema
name: ResourcePolicyList
properties_list: []
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-resource-policy-list-schema.json
slug: incident-manager-resource-policy-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-resource-policy-list-schema.json\",\n  \"title\": \"ResourcePolicyList\",\n  \"description\": \"ResourcePolicyList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"policyDocument\",\n      \"policyId\",\n      \"ramResourceShareRegion\"\n    ],\n    \"properties\": {\n      \"policyDocument\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Policy\"\n          },\n          {\n            \"description\": \"The JSON blob that describes the policy.\"\n          }\n        ]\n      },\n      \"policyId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/PolicyId\"\n          },\n          {\n            \"description\": \"The ID of the resource policy.\"\n\
  \          }\n        ]\n      },\n      \"ramResourceShareRegion\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/String\"\n          },\n          {\n            \"description\": \"The Amazon Web Services Region that policy allows resources to be used in.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"The resource policy that allows Incident Manager to perform actions on resources on your behalf.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-resource-policy-list-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: ResourcePolicyList
---
