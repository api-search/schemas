---
description: Contains information about the resource type <code>RDSDBInstance</code> involved in a GuardDuty finding.
layout: schema
name: RdsDbInstanceDetails
properties_list:
- description: ''
  name: DbInstanceIdentifier
  type: object
- description: ''
  name: Engine
  type: object
- description: ''
  name: EngineVersion
  type: object
- description: ''
  name: DbClusterIdentifier
  type: object
- description: ''
  name: DbInstanceArn
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-rds-db-instance-details-schema.json
slug: guardduty-rds-db-instance-details
source_filename: guardduty-rds-db-instance-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-rds-db-instance-details-schema.json\",\n  \"title\": \"RdsDbInstanceDetails\",\n  \"description\": \"Contains information about the resource type <code>RDSDBInstance</code> involved in a GuardDuty finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DbInstanceIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dbInstanceIdentifier\"\n          },\n          \"description\": \"The identifier associated to the database instance that was involved in the finding.\"\n        }\n      ]\n    },\n    \"Engine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"engine\"\
  \n          },\n          \"description\": \"The database engine of the database instance involved in the finding.\"\n        }\n      ]\n    },\n    \"EngineVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"engineVersion\"\n          },\n          \"description\": \"The version of the database engine that was involved in the finding.\"\n        }\n      ]\n    },\n    \"DbClusterIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dbClusterIdentifier\"\n          },\n          \"description\": \"The identifier of the database cluster that contains the database instance ID involved in the finding.\"\n        }\n      ]\n    },\n    \"DbInstanceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n       \
  \ {\n          \"xml\": {\n            \"name\": \"dbInstanceArn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the database instance involved in the finding.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"Instance tag key-value pairs associated with the database instance ID.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-rds-db-instance-details-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: RdsDbInstanceDetails
---
