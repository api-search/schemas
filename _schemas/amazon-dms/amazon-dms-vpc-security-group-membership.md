---
description: Describes the status of a security group associated with the virtual private cloud (VPC) hosting your replication and DB instances.
layout: schema
name: VpcSecurityGroupMembership
properties_list:
- description: ''
  name: VpcSecurityGroupId
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-vpc-security-group-membership-schema.json
slug: amazon-dms-vpc-security-group-membership
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-vpc-security-group-membership-schema.json\",\n  \"title\": \"VpcSecurityGroupMembership\",\n  \"description\": \"Describes the status of a security group associated with the virtual private cloud (VPC) hosting your replication and DB instances.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcSecurityGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The VPC security group ID.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The status of the VPC security group.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-vpc-security-group-membership-schema.json
tags:
- AWS
- Data Replication
- Database
- Database Migration
- Migration
title: VpcSecurityGroupMembership
---
