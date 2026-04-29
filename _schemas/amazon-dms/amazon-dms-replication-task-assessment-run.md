---
description: <p>Provides information that describes a premigration assessment run that you have started using the <code>StartReplicationTaskAssessmentRun</code> operation.</p> <p>Some of the information appears based on other operations that can return the <code>ReplicationTaskAssessmentRun</code> object.</p>
layout: schema
name: ReplicationTaskAssessmentRun
properties_list:
- description: ''
  name: ReplicationTaskAssessmentRunArn
  type: object
- description: ''
  name: ReplicationTaskArn
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: ReplicationTaskAssessmentRunCreationDate
  type: object
- description: ''
  name: AssessmentProgress
  type: object
- description: ''
  name: LastFailureMessage
  type: object
- description: ''
  name: ServiceAccessRoleArn
  type: object
- description: ''
  name: ResultLocationBucket
  type: object
- description: ''
  name: ResultLocationFolder
  type: object
- description: ''
  name: ResultEncryptionMode
  type: object
- description: ''
  name: ResultKmsKeyArn
  type: object
- description: ''
  name: AssessmentRunName
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-replication-task-assessment-run-schema.json
slug: amazon-dms-replication-task-assessment-run
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-replication-task-assessment-run-schema.json\",\n  \"title\": \"ReplicationTaskAssessmentRun\",\n  \"description\": \"<p>Provides information that describes a premigration assessment run that you have started using the <code>StartReplicationTaskAssessmentRun</code> operation.</p> <p>Some of the information appears based on other operations that can return the <code>ReplicationTaskAssessmentRun</code> object.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReplicationTaskAssessmentRunArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Amazon Resource Name (ARN) of this assessment run.\"\n        }\n      ]\n    },\n    \"ReplicationTaskArn\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"ARN of the migration task associated with this premigration assessment run.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>Assessment run status. </p> <p>This status can have one of the following values:</p> <ul> <li> <p> <code>\\\"cancelling\\\"</code> \\u2013 The assessment run was canceled by the <code>CancelReplicationTaskAssessmentRun</code> operation.</p> </li> <li> <p> <code>\\\"deleting\\\"</code> \\u2013 The assessment run was deleted by the <code>DeleteReplicationTaskAssessmentRun</code> operation.</p> </li> <li> <p> <code>\\\"failed\\\"</code> \\u2013 At least one individual assessment completed with a <code>failed</code> status.</p> </li> <li> <p> <code>\\\"error-provisioning\\\"</code> \\u2013 An internal error occurred while resources were provisioned\
  \ (during <code>provisioning</code> status).</p> </li> <li> <p> <code>\\\"error-executing\\\"</code> \\u2013 An internal error occurred while individual assessments ran (during <code>running</code> status).</p> </li> <li> <p> <code>\\\"invalid state\\\"</code> \\u2013 The assessment run is in an unknown state.</p> </li> <li> <p> <code>\\\"passed\\\"</code> \\u2013 All individual assessments have completed, and none has a <code>failed</code> status.</p> </li> <li> <p> <code>\\\"provisioning\\\"</code> \\u2013 Resources required to run individual assessments are being provisioned.</p> </li> <li> <p> <code>\\\"running\\\"</code> \\u2013 Individual assessments are being run.</p> </li> <li> <p> <code>\\\"starting\\\"</code> \\u2013 The assessment run is starting, but resources are not yet being provisioned for individual assessments.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"ReplicationTaskAssessmentRunCreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\
  \n        },\n        {\n          \"description\": \"Date on which the assessment run was created using the <code>StartReplicationTaskAssessmentRun</code> operation.\"\n        }\n      ]\n    },\n    \"AssessmentProgress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReplicationTaskAssessmentRunProgress\"\n        },\n        {\n          \"description\": \"Indication of the completion progress for the individual assessments specified to run.\"\n        }\n      ]\n    },\n    \"LastFailureMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Last message generated by an individual assessment failure.\"\n        }\n      ]\n    },\n    \"ServiceAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"ARN of the service role used to start the assessment run using\
  \ the <code>StartReplicationTaskAssessmentRun</code> operation. The role must allow the <code>iam:PassRole</code> action.\"\n        }\n      ]\n    },\n    \"ResultLocationBucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Amazon S3 bucket where DMS stores the results of this assessment run.\"\n        }\n      ]\n    },\n    \"ResultLocationFolder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Folder in an Amazon S3 bucket where DMS stores the results of this assessment run.\"\n        }\n      ]\n    },\n    \"ResultEncryptionMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Encryption mode used to encrypt the assessment run results.\"\n        }\n      ]\n    },\n    \"ResultKmsKeyArn\": {\n     \
  \ \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"ARN of the KMS encryption key used to encrypt the assessment run results.\"\n        }\n      ]\n    },\n    \"AssessmentRunName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Unique name of the assessment run.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-replication-task-assessment-run-schema.json
tags:
- AWS
- Data Replication
- Database
- Database Migration
- Migration
title: ReplicationTaskAssessmentRun
---
