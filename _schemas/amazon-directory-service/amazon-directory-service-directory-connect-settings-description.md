---
description: Contains information about an AD Connector directory.
layout: schema
name: DirectoryConnectSettingsDescription
properties_list:
- description: ''
  name: VpcId
  type: object
- description: ''
  name: SubnetIds
  type: object
- description: ''
  name: CustomerUserName
  type: object
- description: ''
  name: SecurityGroupId
  type: object
- description: ''
  name: AvailabilityZones
  type: object
- description: ''
  name: ConnectIps
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-directory-connect-settings-description-schema.json
slug: amazon-directory-service-directory-connect-settings-description
source_filename: amazon-directory-service-directory-connect-settings-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-directory-connect-settings-description-schema.json\",\n  \"title\": \"DirectoryConnectSettingsDescription\",\n  \"description\": \"Contains information about an AD Connector directory.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcId\"\n        },\n        {\n          \"description\": \"The identifier of the VPC that the AD Connector is in.\"\n        }\n      ]\n    },\n    \"SubnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetIds\"\n        },\n        {\n          \"description\": \"A list of subnet identifiers in the VPC that the AD Connector is in.\"\n        }\n      ]\n    },\n    \"CustomerUserName\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/UserName\"\n        },\n        {\n          \"description\": \"The user name of the service account in your self-managed directory.\"\n        }\n      ]\n    },\n    \"SecurityGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroupId\"\n        },\n        {\n          \"description\": \"The security group identifier for the AD Connector directory.\"\n        }\n      ]\n    },\n    \"AvailabilityZones\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AvailabilityZones\"\n        },\n        {\n          \"description\": \"A list of the Availability Zones that the directory is in.\"\n        }\n      ]\n    },\n    \"ConnectIps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddrs\"\n        },\n        {\n          \"description\": \"The IP addresses of the AD Connector servers.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-directory-connect-settings-description-schema.json
tags:
- Active Directory
- Authentication
- AWS
- Directory Services
- Identity Management
title: DirectoryConnectSettingsDescription
---
