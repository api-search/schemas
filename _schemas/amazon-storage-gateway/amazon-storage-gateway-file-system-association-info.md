---
description: Describes the object returned by <code>DescribeFileSystemAssociations</code> that describes a created file system association.
layout: schema
name: FileSystemAssociationInfo
properties_list:
- description: ''
  name: FileSystemAssociationARN
  type: object
- description: ''
  name: LocationARN
  type: object
- description: ''
  name: FileSystemAssociationStatus
  type: object
- description: ''
  name: AuditDestinationARN
  type: object
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: CacheAttributes
  type: object
- description: ''
  name: EndpointNetworkConfiguration
  type: object
- description: ''
  name: FileSystemAssociationStatusDetails
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-file-system-association-info-schema.json
slug: amazon-storage-gateway-file-system-association-info
source_filename: amazon-storage-gateway-file-system-association-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-file-system-association-info-schema.json\",\n  \"title\": \"FileSystemAssociationInfo\",\n  \"description\": \"Describes the object returned by <code>DescribeFileSystemAssociations</code> that describes a created file system association.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileSystemAssociationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileSystemAssociationARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the file system association.\"\n        }\n      ]\n    },\n    \"LocationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileSystemLocationARN\"\n        },\n        {\n          \"description\": \"The ARN of the backend Amazon FSx file\
  \ system used for storing file data. For information, see <a href=\\\"https://docs.aws.amazon.com/fsx/latest/APIReference/API_FileSystem.html\\\">FileSystem</a> in the <i>Amazon FSx API Reference</i>.\"\n        }\n      ]\n    },\n    \"FileSystemAssociationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileSystemAssociationStatus\"\n        },\n        {\n          \"description\": \"The status of the file system association. Valid Values: <code>AVAILABLE</code> | <code>CREATING</code> | <code>DELETING</code> | <code>FORCE_DELETING</code> | <code>UPDATING</code> | <code>ERROR</code> \"\n        }\n      ]\n    },\n    \"AuditDestinationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditDestinationARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the storage used for the audit logs.\"\n        }\n      ]\n    },\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\
  \n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"A list of up to 50 tags assigned to the SMB file share, sorted alphabetically by key name. Each tag is a key-value pair.\"\n        }\n      ]\n    },\n    \"CacheAttributes\": {\n      \"$ref\": \"#/components/schemas/CacheAttributes\"\n    },\n    \"EndpointNetworkConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointNetworkConfiguration\"\n        },\n        {\n          \"description\": \"<p>Specifies network configuration information for the gateway associated with the Amazon FSx file system.</p> <note> <p>If multiple file systems are associated with this gateway, this parameter's <code>IpAddresses</code> field is required.</p> </note>\"\n        }\n      ]\n    },\n    \"FileSystemAssociationStatusDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileSystemAssociationStatusDetails\"\
  \n        },\n        {\n          \"description\": \"An array containing the FileSystemAssociationStatusDetail data type, which provides detailed information on file system association status.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-file-system-association-info-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: FileSystemAssociationInfo
---
