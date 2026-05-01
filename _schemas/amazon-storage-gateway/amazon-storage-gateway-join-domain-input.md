---
description: JoinDomainInput
layout: schema
name: JoinDomainInput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: DomainName
  type: object
- description: ''
  name: OrganizationalUnit
  type: object
- description: ''
  name: DomainControllers
  type: object
- description: ''
  name: TimeoutInSeconds
  type: object
- description: ''
  name: UserName
  type: object
- description: ''
  name: Password
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-join-domain-input-schema.json
slug: amazon-storage-gateway-join-domain-input
source_filename: amazon-storage-gateway-join-domain-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-join-domain-input-schema.json\",\n  \"title\": \"JoinDomainInput\",\n  \"description\": \"JoinDomainInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the gateway. Use the <code>ListGateways</code> operation to return a list of gateways for your account and Amazon Web Services Region.\"\n        }\n      ]\n    },\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain that you want the gateway to join.\"\n        }\n      ]\n    },\n    \"OrganizationalUnit\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationalUnit\"\n        },\n        {\n          \"description\": \"The organizational unit (OU) is a container in an Active Directory that can hold users, groups, computers, and other OUs and this parameter specifies the OU that the gateway will join within the AD domain.\"\n        }\n      ]\n    },\n    \"DomainControllers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Hosts\"\n        },\n        {\n          \"description\": \"List of IPv4 addresses, NetBIOS names, or host names of your domain server. If you need to specify the port number include it after the colon (\\u201c:\\u201d). For example, <code>mydc.mydomain.com:389</code>.\"\n        }\n      ]\n    },\n    \"TimeoutInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeoutInSeconds\"\n        },\n        {\n          \"description\": \"Specifies the time in seconds,\
  \ in which the <code>JoinDomain</code> operation must complete. The default is 20 seconds.\"\n        }\n      ]\n    },\n    \"UserName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainUserName\"\n        },\n        {\n          \"description\": \"Sets the user name of user who has permission to add the gateway to the Active Directory domain. The domain user account should be enabled to join computers to the domain. For example, you can use the domain administrator account or an account with delegated permissions to join computers to the domain.\"\n        }\n      ]\n    },\n    \"Password\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainUserPassword\"\n        },\n        {\n          \"description\": \"Sets the password of the user who has permission to add the gateway to the Active Directory domain.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GatewayARN\",\n    \"DomainName\",\n    \"UserName\"\
  ,\n    \"Password\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-join-domain-input-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: JoinDomainInput
---
