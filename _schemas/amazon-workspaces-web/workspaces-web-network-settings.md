---
description: A network settings resource that can be associated with a web portal. Once associated with a web portal, network settings define how streaming instances will connect with your specified VPC.
layout: schema
name: NetworkSettings
properties_list:
- description: ''
  name: associatedPortalArns
  type: object
- description: ''
  name: networkSettingsArn
  type: object
- description: ''
  name: securityGroupIds
  type: object
- description: ''
  name: subnetIds
  type: object
- description: ''
  name: vpcId
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-network-settings-schema.json
slug: workspaces-web-network-settings
source_filename: workspaces-web-network-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"networkSettingsArn\"\n  ],\n  \"properties\": {\n    \"associatedPortalArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnList\"\n        },\n        {\n          \"description\": \"A list of web portal ARNs that this network settings is associated with.\"\n        }\n      ]\n    },\n    \"networkSettingsArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the network settings.\"\n        }\n      ]\n    },\n    \"securityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroupIdList\"\n        },\n        {\n          \"description\": \"One or more security groups used to control access from streaming instances to your VPC. \"\n        }\n      ]\n    },\n    \"subnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetIdList\"\
  \n        },\n        {\n          \"description\": \"The subnets in which network interfaces are created to connect streaming instances to your VPC. At least two of these subnets must be in different availability zones.\"\n        }\n      ]\n    },\n    \"vpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcId\"\n        },\n        {\n          \"description\": \"The VPC that streaming instances will connect to.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A network settings resource that can be associated with a web portal. Once associated with a web portal, network settings define how streaming instances will connect with your specified VPC. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NetworkSettings\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-network-settings-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-network-settings-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: NetworkSettings
---
