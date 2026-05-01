---
description: In response to a request by the <code>DescribeReplicationSubnetGroups</code> operation, this object identifies a subnet by its given Availability Zone, subnet identifier, and status.
layout: schema
name: Subnet
properties_list:
- description: ''
  name: SubnetIdentifier
  type: object
- description: ''
  name: SubnetAvailabilityZone
  type: object
- description: ''
  name: SubnetStatus
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-subnet-schema.json
slug: amazon-dms-subnet
source_filename: amazon-dms-subnet-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-subnet-schema.json\",\n  \"title\": \"Subnet\",\n  \"description\": \"In response to a request by the <code>DescribeReplicationSubnetGroups</code> operation, this object identifies a subnet by its given Availability Zone, subnet identifier, and status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SubnetIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The subnet identifier.\"\n        }\n      ]\n    },\n    \"SubnetAvailabilityZone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AvailabilityZone\"\n        },\n        {\n          \"description\": \"The Availability Zone of the subnet.\"\n        }\n      ]\n    },\n    \"SubnetStatus\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The status of the subnet.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-subnet-schema.json
tags:
- Data Replication
- Database
- Database Migration
- Migration
title: Subnet
---
