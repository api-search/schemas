---
description: Describes a subnet group in response to a request by the <code>DescribeReplicationSubnetGroups</code> operation.
layout: schema
name: ReplicationSubnetGroup
properties_list:
- description: ''
  name: ReplicationSubnetGroupIdentifier
  type: object
- description: ''
  name: ReplicationSubnetGroupDescription
  type: object
- description: ''
  name: VpcId
  type: object
- description: ''
  name: SubnetGroupStatus
  type: object
- description: ''
  name: Subnets
  type: object
- description: ''
  name: SupportedNetworkTypes
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-replication-subnet-group-schema.json
slug: amazon-dms-replication-subnet-group
source_filename: amazon-dms-replication-subnet-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-replication-subnet-group-schema.json\",\n  \"title\": \"ReplicationSubnetGroup\",\n  \"description\": \"Describes a subnet group in response to a request by the <code>DescribeReplicationSubnetGroups</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReplicationSubnetGroupIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The identifier of the replication instance subnet group.\"\n        }\n      ]\n    },\n    \"ReplicationSubnetGroupDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A description for the replication subnet group.\"\n        }\n      ]\n    },\n    \"VpcId\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ID of the VPC.\"\n        }\n      ]\n    },\n    \"SubnetGroupStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The status of the subnet group.\"\n        }\n      ]\n    },\n    \"Subnets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetList\"\n        },\n        {\n          \"description\": \"The subnets that are in the subnet group.\"\n        }\n      ]\n    },\n    \"SupportedNetworkTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \"The IP addressing protocol supported by the subnet group. This is used by a replication instance with values such as IPv4 only or Dual-stack that supports both IPv4 and IPv6\
  \ addressing. IPv6 only is not yet supported.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-replication-subnet-group-schema.json
tags:
- AWS
- Data Replication
- Database
- Database Migration
- Migration
title: ReplicationSubnetGroup
---
