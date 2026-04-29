---
description: DescribeAccountResult schema from Amazon WorkSpaces API
layout: schema
name: DescribeAccountResult
properties_list:
- description: ''
  name: DedicatedTenancySupport
  type: object
- description: ''
  name: DedicatedTenancyManagementCidrRange
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-account-result-schema.json
slug: workspaces-describe-account-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"DedicatedTenancySupport\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DedicatedTenancySupportResultEnum\"\n        },\n        {\n          \"description\": \"The status of BYOL (whether BYOL is enabled or disabled).\"\n        }\n      ]\n    },\n    \"DedicatedTenancyManagementCidrRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DedicatedTenancyManagementCidrRange\"\n        },\n        {\n          \"description\": \"<p>The IP address range, specified as an IPv4 CIDR block, used for the management network interface.</p> <p>The management network interface is connected to a secure Amazon WorkSpaces management network. It is used for interactive streaming of the WorkSpace desktop to Amazon WorkSpaces clients, and to allow Amazon WorkSpaces to manage the WorkSpace.</p>\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"DescribeAccountResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-account-result-schema.json\",\n  \"description\": \"DescribeAccountResult schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-account-result-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeAccountResult
---
