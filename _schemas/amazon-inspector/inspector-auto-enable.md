---
description: Represents which scan types are automatically enabled for new members of your Amazon Inspector organization.
layout: schema
name: AutoEnable
properties_list:
- description: ''
  name: ec2
  type: object
- description: ''
  name: ecr
  type: object
- description: ''
  name: lambda
  type: object
- description: ''
  name: lambdaCode
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-auto-enable-schema.json
slug: inspector-auto-enable
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-auto-enable-schema.json\",\n  \"title\": \"AutoEnable\",\n  \"description\": \"Represents which scan types are automatically enabled for new members of your Amazon Inspector organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ec2\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Represents whether Amazon EC2 scans are automatically enabled for new members of your Amazon Inspector organization.\"\n        }\n      ]\n    },\n    \"ecr\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Represents whether Amazon ECR scans are automatically enabled for new members of your Amazon Inspector organization.\"\
  \n        }\n      ]\n    },\n    \"lambda\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Represents whether AWS Lambda standard scans are automatically enabled for new members of your Amazon Inspector organization. \"\n        }\n      ]\n    },\n    \"lambdaCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Represents whether AWS Lambda code scans are automatically enabled for new members of your Amazon Inspector organization. <pre><code> &lt;/p&gt; </code></pre>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ec2\",\n    \"ecr\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-auto-enable-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: AutoEnable
---
