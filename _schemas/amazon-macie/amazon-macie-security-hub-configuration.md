---
description: Specifies configuration settings that determine which findings are published to Security Hub automatically. For information about how Macie publishes findings to Security Hub, see <a href="https://docs.aws.amazon.com/macie/latest/user/securityhub-integration.html">Amazon Macie integration with Security Hub</a> in the <i>Amazon Macie User Guide</i>.
layout: schema
name: SecurityHubConfiguration
properties_list:
- description: ''
  name: publishClassificationFindings
  type: object
- description: ''
  name: publishPolicyFindings
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-security-hub-configuration-schema.json
slug: amazon-macie-security-hub-configuration
source_filename: amazon-macie-security-hub-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-security-hub-configuration-schema.json\",\n  \"title\": \"SecurityHubConfiguration\",\n  \"description\": \"Specifies configuration settings that determine which findings are published to Security Hub automatically. For information about how Macie publishes findings to Security Hub, see <a href=\\\"https://docs.aws.amazon.com/macie/latest/user/securityhub-integration.html\\\">Amazon Macie integration with Security Hub</a> in the <i>Amazon Macie User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"publishClassificationFindings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether to publish sensitive data findings to Security Hub. If you set this value to true, Amazon\
  \ Macie automatically publishes all sensitive data findings that weren't suppressed by a findings filter. The default value is false.\"\n        }\n      ]\n    },\n    \"publishPolicyFindings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether to publish policy findings to Security Hub. If you set this value to true, Amazon Macie automatically publishes all new and updated policy findings that weren't suppressed by a findings filter. The default value is true.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"publishPolicyFindings\",\n    \"publishClassificationFindings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-security-hub-configuration-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SecurityHubConfiguration
---
