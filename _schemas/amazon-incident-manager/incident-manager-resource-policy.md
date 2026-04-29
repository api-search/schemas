---
description: The resource policy that allows Incident Manager to perform actions on resources on your behalf.
layout: schema
name: ResourcePolicy
properties_list:
- description: ''
  name: policyDocument
  type: object
- description: ''
  name: policyId
  type: object
- description: ''
  name: ramResourceShareRegion
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-resource-policy-schema.json
slug: incident-manager-resource-policy
source_filename: incident-manager-resource-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-resource-policy-schema.json\",\n  \"title\": \"ResourcePolicy\",\n  \"description\": \"The resource policy that allows Incident Manager to perform actions on resources on your behalf.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policyDocument\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Policy\"\n        },\n        {\n          \"description\": \"The JSON blob that describes the policy.\"\n        }\n      ]\n    },\n    \"policyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyId\"\n        },\n        {\n          \"description\": \"The ID of the resource policy.\"\n        }\n      ]\n    },\n    \"ramResourceShareRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\
  \n        },\n        {\n          \"description\": \"The Amazon Web Services Region that policy allows resources to be used in.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"policyDocument\",\n    \"policyId\",\n    \"ramResourceShareRegion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-resource-policy-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: ResourcePolicy
---
