---
description: AssociateFileSystemInput schema from Amazon Storage Gateway API
layout: schema
name: AssociateFileSystemInput
properties_list:
- description: ''
  name: UserName
  type: object
- description: ''
  name: Password
  type: object
- description: ''
  name: ClientToken
  type: object
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: LocationARN
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: AuditDestinationARN
  type: object
- description: ''
  name: CacheAttributes
  type: object
- description: ''
  name: EndpointNetworkConfiguration
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-associate-file-system-input-schema.json
slug: amazon-storage-gateway-associate-file-system-input
source_filename: amazon-storage-gateway-associate-file-system-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-associate-file-system-input-schema.json\",\n  \"title\": \"AssociateFileSystemInput\",\n  \"description\": \"AssociateFileSystemInput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainUserName\"\n        },\n        {\n          \"description\": \"The user name of the user credential that has permission to access the root share D$ of the Amazon FSx file system. The user account must belong to the Amazon FSx delegated admin user group.\"\n        }\n      ]\n    },\n    \"Password\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainUserPassword\"\n        },\n        {\n          \"description\": \"The\
  \ password of the user credential.\"\n        }\n      ]\n    },\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"A unique string value that you supply that is used by the FSx File Gateway to ensure idempotent file system association creation.\"\n        }\n      ]\n    },\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"LocationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileSystemLocationARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Amazon FSx file system to associate with the FSx File Gateway.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"A list of up to 50 tags that can be assigned to the file system association.\
  \ Each tag is a key-value pair.\"\n        }\n      ]\n    },\n    \"AuditDestinationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditDestinationARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the storage used for the audit logs.\"\n        }\n      ]\n    },\n    \"CacheAttributes\": {\n      \"$ref\": \"#/components/schemas/CacheAttributes\"\n    },\n    \"EndpointNetworkConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointNetworkConfiguration\"\n        },\n        {\n          \"description\": \"<p>Specifies the network configuration information for the gateway associated with the Amazon FSx file system.</p> <note> <p>If multiple file systems are associated with this gateway, this parameter's <code>IpAddresses</code> field is required.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserName\",\n    \"Password\",\n    \"ClientToken\"\
  ,\n    \"GatewayARN\",\n    \"LocationARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-associate-file-system-input-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: AssociateFileSystemInput
---
