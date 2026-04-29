---
description: Contains information for the <a>ConnectDirectory</a> operation when an AD Connector directory is being created.
layout: schema
name: DirectoryConnectSettings
properties_list:
- description: ''
  name: VpcId
  type: object
- description: ''
  name: SubnetIds
  type: object
- description: ''
  name: CustomerDnsIps
  type: object
- description: ''
  name: CustomerUserName
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-directory-connect-settings-schema.json
slug: amazon-directory-service-directory-connect-settings
source_filename: amazon-directory-service-directory-connect-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-directory-connect-settings-schema.json\",\n  \"title\": \"DirectoryConnectSettings\",\n  \"description\": \"Contains information for the <a>ConnectDirectory</a> operation when an AD Connector directory is being created.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcId\"\n        },\n        {\n          \"description\": \"The identifier of the VPC in which the AD Connector is created.\"\n        }\n      ]\n    },\n    \"SubnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetIds\"\n        },\n        {\n          \"description\": \"A list of subnet identifiers in the VPC in which the AD Connector is created.\"\n        }\n      ]\n\
  \    },\n    \"CustomerDnsIps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DnsIpAddrs\"\n        },\n        {\n          \"description\": \"A list of one or more IP addresses of DNS servers or domain controllers in your self-managed directory.\"\n        }\n      ]\n    },\n    \"CustomerUserName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserName\"\n        },\n        {\n          \"description\": \"<p>The user name of an account in your self-managed directory that is used to connect to the directory. This account must have the following permissions:</p> <ul> <li> <p>Read users and groups</p> </li> <li> <p>Create computer objects</p> </li> <li> <p>Join computers to the domain</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VpcId\",\n    \"SubnetIds\",\n    \"CustomerDnsIps\",\n    \"CustomerUserName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-directory-connect-settings-schema.json
tags:
- Active Directory
- Authentication
- AWS
- Directory Services
- Identity Management
title: DirectoryConnectSettings
---
