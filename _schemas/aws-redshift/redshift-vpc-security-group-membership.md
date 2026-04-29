---
description: Describes the members of a VPC security group.
layout: schema
name: VpcSecurityGroupMembership
properties_list:
- description: ''
  name: VpcSecurityGroupId
  type: object
- description: ''
  name: Status
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-vpc-security-group-membership-schema.json
slug: redshift-vpc-security-group-membership
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcSecurityGroupId\": {},\n    \"Status\": {}\n  },\n  \"description\": \"Describes the members of a VPC security group.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-vpc-security-group-membership-schema.json\",\n  \"title\": \"VpcSecurityGroupMembership\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-vpc-security-group-membership-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: VpcSecurityGroupMembership
---
