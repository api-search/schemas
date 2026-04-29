---
description: A structure containing information about how this workspace works with IAM Identity Center.
layout: schema
name: AwsSsoAuthentication
properties_list:
- description: ''
  name: ssoClientId
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-aws-sso-authentication-schema.json
slug: amazon-managed-grafana-aws-sso-authentication
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-aws-sso-authentication-schema.json\",\n  \"title\": \"AwsSsoAuthentication\",\n  \"description\": \"A structure containing information about how this workspace works with IAM Identity Center. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ssoClientId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SSOClientId\"\n        },\n        {\n          \"description\": \"The ID of the IAM Identity Center-managed application that is created by Amazon Managed Grafana.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-aws-sso-authentication-schema.json
tags:
- AWS
- Dashboards
- Monitoring
- Observability
- Visualization
title: AwsSsoAuthentication
---
