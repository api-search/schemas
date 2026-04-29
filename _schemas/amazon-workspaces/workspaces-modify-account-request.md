---
description: ModifyAccountRequest schema from Amazon WorkSpaces API
layout: schema
name: ModifyAccountRequest
properties_list:
- description: ''
  name: DedicatedTenancySupport
  type: object
- description: ''
  name: DedicatedTenancyManagementCidrRange
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-modify-account-request-schema.json
slug: workspaces-modify-account-request
source_filename: workspaces-modify-account-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"ModifyAccountRequest\",\n  \"properties\": {\n    \"DedicatedTenancySupport\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DedicatedTenancySupportEnum\"\n        },\n        {\n          \"description\": \"The status of BYOL.\"\n        }\n      ]\n    },\n    \"DedicatedTenancyManagementCidrRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DedicatedTenancyManagementCidrRange\"\n        },\n        {\n          \"description\": \"The IP address range, specified as an IPv4 CIDR block, for the management network interface. Specify an IP address range that is compatible with your network and in CIDR notation (that is, specify the range as an IPv4 CIDR block). The CIDR block size must be /16 (for example, 203.0.113.25/16). It must also be specified as available by the <code>ListAvailableManagementCidrRanges</code> operation.\"\n        }\n      ]\n    }\n  },\n  \"$schema\"\
  : \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-modify-account-request-schema.json\",\n  \"description\": \"ModifyAccountRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-modify-account-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ModifyAccountRequest
---
