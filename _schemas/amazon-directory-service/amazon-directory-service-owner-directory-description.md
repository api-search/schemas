---
description: Describes the directory owner account details that have been shared to the directory consumer account.
layout: schema
name: OwnerDirectoryDescription
properties_list:
- description: ''
  name: DirectoryId
  type: object
- description: ''
  name: AccountId
  type: object
- description: ''
  name: DnsIpAddrs
  type: object
- description: ''
  name: VpcSettings
  type: object
- description: ''
  name: RadiusSettings
  type: object
- description: ''
  name: RadiusStatus
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-owner-directory-description-schema.json
slug: amazon-directory-service-owner-directory-description
source_filename: amazon-directory-service-owner-directory-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-owner-directory-description-schema.json\",\n  \"title\": \"OwnerDirectoryDescription\",\n  \"description\": \"Describes the directory owner account details that have been shared to the directory consumer account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"Identifier of the Managed Microsoft AD directory in the directory owner account.\"\n        }\n      ]\n    },\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerId\"\n        },\n        {\n          \"description\": \"Identifier of the directory owner account.\"\n        }\n      ]\n    },\n  \
  \  \"DnsIpAddrs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DnsIpAddrs\"\n        },\n        {\n          \"description\": \"IP address of the directory\\u2019s domain controllers.\"\n        }\n      ]\n    },\n    \"VpcSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryVpcSettingsDescription\"\n        },\n        {\n          \"description\": \"Information about the VPC settings for the directory.\"\n        }\n      ]\n    },\n    \"RadiusSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RadiusSettings\"\n        },\n        {\n          \"description\": \"A <a>RadiusSettings</a> object that contains information about the RADIUS server.\"\n        }\n      ]\n    },\n    \"RadiusStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RadiusStatus\"\n        },\n        {\n          \"description\": \"Information about the status of\
  \ the RADIUS server.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-owner-directory-description-schema.json
tags:
- Active Directory
- Authentication
- AWS
- Directory Services
- Identity Management
title: OwnerDirectoryDescription
---
