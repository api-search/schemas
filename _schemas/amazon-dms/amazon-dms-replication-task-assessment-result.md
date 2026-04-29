---
description: The task assessment report in JSON format.
layout: schema
name: ReplicationTaskAssessmentResult
properties_list:
- description: ''
  name: ReplicationTaskIdentifier
  type: object
- description: ''
  name: ReplicationTaskArn
  type: object
- description: ''
  name: ReplicationTaskLastAssessmentDate
  type: object
- description: ''
  name: AssessmentStatus
  type: object
- description: ''
  name: AssessmentResultsFile
  type: object
- description: ''
  name: AssessmentResults
  type: object
- description: ''
  name: S3ObjectUrl
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-replication-task-assessment-result-schema.json
slug: amazon-dms-replication-task-assessment-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-replication-task-assessment-result-schema.json\",\n  \"title\": \"ReplicationTaskAssessmentResult\",\n  \"description\": \" The task assessment report in JSON format. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReplicationTaskIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The replication task identifier of the task on which the task assessment was run. \"\n        }\n      ]\n    },\n    \"ReplicationTaskArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the replication task. \"\n        }\n      ]\n    },\n    \"ReplicationTaskLastAssessmentDate\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"The date the task assessment was completed. \"\n        }\n      ]\n    },\n    \"AssessmentStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The status of the task assessment. \"\n        }\n      ]\n    },\n    \"AssessmentResultsFile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The file containing the results of the task assessment. \"\n        }\n      ]\n    },\n    \"AssessmentResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p> The task assessment results in JSON format. </p> <p>The response object only contains this field if you provide <a>DescribeReplicationTaskAssessmentResultsMessage$ReplicationTaskArn</a>\
  \ in the request.</p>\"\n        }\n      ]\n    },\n    \"S3ObjectUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p> The URL of the S3 object containing the task assessment results. </p> <p>The response object only contains this field if you provide <a>DescribeReplicationTaskAssessmentResultsMessage$ReplicationTaskArn</a> in the request.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-replication-task-assessment-result-schema.json
tags:
- AWS
- Data Replication
- Database
- Database Migration
- Migration
title: ReplicationTaskAssessmentResult
---
