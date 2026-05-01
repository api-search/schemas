---
description: Contains VPC information for the <a>CreateDirectory</a> or <a>CreateMicrosoftAD</a> operation.
layout: schema
name: DirectoryVpcSettings
properties_list:
- description: ''
  name: VpcId
  type: object
- description: ''
  name: SubnetIds
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-directory-vpc-settings-schema.json
slug: amazon-directory-service-directory-vpc-settings
source_filename: amazon-directory-service-directory-vpc-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-directory-vpc-settings-schema.json\",\n  \"title\": \"DirectoryVpcSettings\",\n  \"description\": \"Contains VPC information for the <a>CreateDirectory</a> or <a>CreateMicrosoftAD</a> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcId\"\n        },\n        {\n          \"description\": \"The identifier of the VPC in which to create the directory.\"\n        }\n      ]\n    },\n    \"SubnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetIds\"\n        },\n        {\n          \"description\": \"The identifiers of the subnets for the directory servers. The two subnets must be in different Availability Zones. Directory Service\
  \ creates a directory server and a DNS server in each of these subnets.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VpcId\",\n    \"SubnetIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-directory-vpc-settings-schema.json
tags:
- Active Directory
- Authentication
- Directory Services
- Identity Management
title: DirectoryVpcSettings
---
