---
description: In response to the <code>DescribeOrderableReplicationInstances</code> operation, this object describes an available replication instance. This description includes the replication instance's type, engine version, and allocated storage.
layout: schema
name: OrderableReplicationInstance
properties_list:
- description: ''
  name: EngineVersion
  type: object
- description: ''
  name: ReplicationInstanceClass
  type: object
- description: ''
  name: StorageType
  type: object
- description: ''
  name: MinAllocatedStorage
  type: object
- description: ''
  name: MaxAllocatedStorage
  type: object
- description: ''
  name: DefaultAllocatedStorage
  type: object
- description: ''
  name: IncludedAllocatedStorage
  type: object
- description: ''
  name: AvailabilityZones
  type: object
- description: ''
  name: ReleaseStatus
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-orderable-replication-instance-schema.json
slug: amazon-dms-orderable-replication-instance
source_filename: amazon-dms-orderable-replication-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-orderable-replication-instance-schema.json\",\n  \"title\": \"OrderableReplicationInstance\",\n  \"description\": \"In response to the <code>DescribeOrderableReplicationInstances</code> operation, this object describes an available replication instance. This description includes the replication instance's type, engine version, and allocated storage.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EngineVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The version of the replication engine.\"\n        }\n      ]\n    },\n    \"ReplicationInstanceClass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"\
  <p>The compute and memory capacity of the replication instance as defined for the specified replication instance class. For example to specify the instance class dms.c4.large, set this parameter to <code>\\\"dms.c4.large\\\"</code>.</p> <p>For more information on the settings and capacities for the available replication instance classes, see <a href=\\\"https://docs.aws.amazon.com/dms/latest/userguide/CHAP_ReplicationInstance.html#CHAP_ReplicationInstance.InDepth\\\"> Selecting the right DMS replication instance for your migration</a>. </p>\"\n        }\n      ]\n    },\n    \"StorageType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The type of storage used by the replication instance.\"\n        }\n      ]\n    },\n    \"MinAllocatedStorage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The minimum\
  \ amount of storage (in gigabytes) that can be allocated for the replication instance.\"\n        }\n      ]\n    },\n    \"MaxAllocatedStorage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The minimum amount of storage (in gigabytes) that can be allocated for the replication instance.\"\n        }\n      ]\n    },\n    \"DefaultAllocatedStorage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The default amount of storage (in gigabytes) that is allocated for the replication instance.\"\n        }\n      ]\n    },\n    \"IncludedAllocatedStorage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The amount of storage (in gigabytes) that is allocated for the replication instance.\"\n        }\n      ]\n    },\n\
  \    \"AvailabilityZones\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AvailabilityZonesList\"\n        },\n        {\n          \"description\": \"List of Availability Zones for this replication instance.\"\n        }\n      ]\n    },\n    \"ReleaseStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReleaseStatusValues\"\n        },\n        {\n          \"description\": \"<p>The value returned when the specified <code>EngineVersion</code> of the replication instance is in Beta or test mode. This indicates some features might not work as expected.</p> <note> <p>DMS supports the <code>ReleaseStatus</code> parameter in versions 3.1.4 and later.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-orderable-replication-instance-schema.json
tags:
- AWS
- Data Replication
- Database
- Database Migration
- Migration
title: OrderableReplicationInstance
---
