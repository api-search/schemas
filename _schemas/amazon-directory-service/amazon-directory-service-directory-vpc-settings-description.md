---
description: Contains information about the directory.
layout: schema
name: DirectoryVpcSettingsDescription
properties_list:
- description: ''
  name: VpcId
  type: object
- description: ''
  name: SubnetIds
  type: object
- description: ''
  name: SecurityGroupId
  type: object
- description: ''
  name: AvailabilityZones
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-directory-vpc-settings-description-schema.json
slug: amazon-directory-service-directory-vpc-settings-description
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-directory-vpc-settings-description-schema.json\",\n  \"title\": \"DirectoryVpcSettingsDescription\",\n  \"description\": \"Contains information about the directory.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcId\"\n        },\n        {\n          \"description\": \"The identifier of the VPC that the directory is in.\"\n        }\n      ]\n    },\n    \"SubnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetIds\"\n        },\n        {\n          \"description\": \"The identifiers of the subnets for the directory servers.\"\n        }\n      ]\n    },\n    \"SecurityGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/SecurityGroupId\"\n        },\n        {\n          \"description\": \"The domain controller security group identifier for the directory.\"\n        }\n      ]\n    },\n    \"AvailabilityZones\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AvailabilityZones\"\n        },\n        {\n          \"description\": \"The list of Availability Zones that the directory is in.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-directory-vpc-settings-description-schema.json
tags:
- Active Directory
- Authentication
- AWS
- Directory Services
- Identity Management
title: DirectoryVpcSettingsDescription
---
