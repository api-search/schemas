---
description: Provides information that describes a replication task created by the <code>CreateReplicationTask</code> operation.
layout: schema
name: ReplicationTask
properties_list:
- description: ''
  name: ReplicationTaskIdentifier
  type: object
- description: ''
  name: SourceEndpointArn
  type: object
- description: ''
  name: TargetEndpointArn
  type: object
- description: ''
  name: ReplicationInstanceArn
  type: object
- description: ''
  name: MigrationType
  type: object
- description: ''
  name: TableMappings
  type: object
- description: ''
  name: ReplicationTaskSettings
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: LastFailureMessage
  type: object
- description: ''
  name: StopReason
  type: object
- description: ''
  name: ReplicationTaskCreationDate
  type: object
- description: ''
  name: ReplicationTaskStartDate
  type: object
- description: ''
  name: CdcStartPosition
  type: object
- description: ''
  name: CdcStopPosition
  type: object
- description: ''
  name: RecoveryCheckpoint
  type: object
- description: ''
  name: ReplicationTaskArn
  type: object
- description: ''
  name: ReplicationTaskStats
  type: object
- description: ''
  name: TaskData
  type: object
- description: ''
  name: TargetReplicationInstanceArn
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-replication-task-schema.json
slug: amazon-dms-replication-task
source_filename: amazon-dms-replication-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-replication-task-schema.json\",\n  \"title\": \"ReplicationTask\",\n  \"description\": \"Provides information that describes a replication task created by the <code>CreateReplicationTask</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReplicationTaskIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The user-assigned replication task identifier or name.</p> <p>Constraints:</p> <ul> <li> <p>Must contain 1-255 alphanumeric characters or hyphens.</p> </li> <li> <p>First character must be a letter.</p> </li> <li> <p>Cannot end with a hyphen or contain two consecutive hyphens.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"SourceEndpointArn\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that uniquely identifies the endpoint.\"\n        }\n      ]\n    },\n    \"TargetEndpointArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ARN that uniquely identifies the endpoint.\"\n        }\n      ]\n    },\n    \"ReplicationInstanceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ARN of the replication instance.\"\n        }\n      ]\n    },\n    \"MigrationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MigrationTypeValue\"\n        },\n        {\n          \"description\": \"The type of migration.\"\n        }\n      ]\n    },\n    \"TableMappings\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Table mappings specified in the task.\"\n        }\n      ]\n    },\n    \"ReplicationTaskSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The settings for the replication task.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The status of the replication task. This response parameter can return one of the following values:</p> <ul> <li> <p> <code>\\\"moving\\\"</code> \\u2013 The task is being moved in response to running the <a href=\\\"https://docs.aws.amazon.com/dms/latest/APIReference/API_MoveReplicationTask.html\\\"> <code>MoveReplicationTask</code> </a> operation.</p> </li> <li> <p> <code>\\\"creating\\\"</code> \\u2013 The task is being created in response\
  \ to running the <a href=\\\"https://docs.aws.amazon.com/dms/latest/APIReference/API_CreateReplicationTask.html\\\"> <code>CreateReplicationTask</code> </a> operation.</p> </li> <li> <p> <code>\\\"deleting\\\"</code> \\u2013 The task is being deleted in response to running the <a href=\\\"https://docs.aws.amazon.com/dms/latest/APIReference/API_DeleteReplicationTask.html\\\"> <code>DeleteReplicationTask</code> </a> operation.</p> </li> <li> <p> <code>\\\"failed\\\"</code> \\u2013 The task failed to successfully complete the database migration in response to running the <a href=\\\"https://docs.aws.amazon.com/dms/latest/APIReference/API_StartReplicationTask.html\\\"> <code>StartReplicationTask</code> </a> operation.</p> </li> <li> <p> <code>\\\"failed-move\\\"</code> \\u2013 The task failed to move in response to running the <a href=\\\"https://docs.aws.amazon.com/dms/latest/APIReference/API_MoveReplicationTask.html\\\"> <code>MoveReplicationTask</code> </a> operation.</p> </li> <li> <p>\
  \ <code>\\\"modifying\\\"</code> \\u2013 The task definition is being modified in response to running the <a href=\\\"https://docs.aws.amazon.com/dms/latest/APIReference/API_ModifyReplicationTask.html\\\"> <code>ModifyReplicationTask</code> </a> operation.</p> </li> <li> <p> <code>\\\"ready\\\"</code> \\u2013 The task is in a <code>ready</code> state where it can respond to other task operations, such as <a href=\\\"https://docs.aws.amazon.com/dms/latest/APIReference/API_StartReplicationTask.html\\\"> <code>StartReplicationTask</code> </a> or <a href=\\\"https://docs.aws.amazon.com/dms/latest/APIReference/API_DeleteReplicationTask.html\\\"> <code>DeleteReplicationTask</code> </a>. </p> </li> <li> <p> <code>\\\"running\\\"</code> \\u2013 The task is performing a database migration in response to running the <a href=\\\"https://docs.aws.amazon.com/dms/latest/APIReference/API_StartReplicationTask.html\\\"> <code>StartReplicationTask</code> </a> operation.</p> </li> <li> <p> <code>\\\"starting\\\
  \"</code> \\u2013 The task is preparing to perform a database migration in response to running the <a href=\\\"https://docs.aws.amazon.com/dms/latest/APIReference/API_StartReplicationTask.html\\\"> <code>StartReplicationTask</code> </a> operation.</p> </li> <li> <p> <code>\\\"stopped\\\"</code> \\u2013 The task has stopped in response to running the <a href=\\\"https://docs.aws.amazon.com/dms/latest/APIReference/API_StopReplicationTask.html\\\"> <code>StopReplicationTask</code> </a> operation.</p> </li> <li> <p> <code>\\\"stopping\\\"</code> \\u2013 The task is preparing to stop in response to running the <a href=\\\"https://docs.aws.amazon.com/dms/latest/APIReference/API_StopReplicationTask.html\\\"> <code>StopReplicationTask</code> </a> operation.</p> </li> <li> <p> <code>\\\"testing\\\"</code> \\u2013 The database migration specified for this task is being tested in response to running either the <a href=\\\"https://docs.aws.amazon.com/dms/latest/APIReference/API_StartReplicationTaskAssessmentRun.html\\\
  \"> <code>StartReplicationTaskAssessmentRun</code> </a> or the <a href=\\\"https://docs.aws.amazon.com/dms/latest/APIReference/API_StartReplicationTaskAssessment.html\\\"> <code>StartReplicationTaskAssessment</code> </a> operation.</p> <note> <p> <a href=\\\"https://docs.aws.amazon.com/dms/latest/APIReference/API_StartReplicationTaskAssessmentRun.html\\\"> <code>StartReplicationTaskAssessmentRun</code> </a> is an improved premigration task assessment operation. The <a href=\\\"https://docs.aws.amazon.com/dms/latest/APIReference/API_StartReplicationTaskAssessment.html\\\"> <code>StartReplicationTaskAssessment</code> </a> operation assesses data type compatibility only between the source and target database of a given migration task. In contrast, <a href=\\\"https://docs.aws.amazon.com/dms/latest/APIReference/API_StartReplicationTaskAssessmentRun.html\\\"> <code>StartReplicationTaskAssessmentRun</code> </a> enables you to specify a variety of premigration task assessments in addition to\
  \ data type compatibility. These assessments include ones for the validity of primary key definitions and likely issues with database migration performance, among others.</p> </note> </li> </ul>\"\n        }\n      ]\n    },\n    \"LastFailureMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The last error (failure) message generated for the replication task.\"\n        }\n      ]\n    },\n    \"StopReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The reason the replication task was stopped. This response parameter can return one of the following values:</p> <ul> <li> <p> <code>\\\"Stop Reason NORMAL\\\"</code> </p> </li> <li> <p> <code>\\\"Stop Reason RECOVERABLE_ERROR\\\"</code> </p> </li> <li> <p> <code>\\\"Stop Reason FATAL_ERROR\\\"</code> </p> </li> <li> <p> <code>\\\"Stop Reason\
  \ FULL_LOAD_ONLY_FINISHED\\\"</code> </p> </li> <li> <p> <code>\\\"Stop Reason STOPPED_AFTER_FULL_LOAD\\\"</code> \\u2013 Full load completed, with cached changes not applied</p> </li> <li> <p> <code>\\\"Stop Reason STOPPED_AFTER_CACHED_EVENTS\\\"</code> \\u2013 Full load completed, with cached changes applied</p> </li> <li> <p> <code>\\\"Stop Reason EXPRESS_LICENSE_LIMITS_REACHED\\\"</code> </p> </li> <li> <p> <code>\\\"Stop Reason STOPPED_AFTER_DDL_APPLY\\\"</code> \\u2013 User-defined stop task after DDL applied</p> </li> <li> <p> <code>\\\"Stop Reason STOPPED_DUE_TO_LOW_MEMORY\\\"</code> </p> </li> <li> <p> <code>\\\"Stop Reason STOPPED_DUE_TO_LOW_DISK\\\"</code> </p> </li> <li> <p> <code>\\\"Stop Reason STOPPED_AT_SERVER_TIME\\\"</code> \\u2013 User-defined server time for stopping task</p> </li> <li> <p> <code>\\\"Stop Reason STOPPED_AT_COMMIT_TIME\\\"</code> \\u2013 User-defined commit time for stopping task</p> </li> <li> <p> <code>\\\"Stop Reason RECONFIGURATION_RESTART\\\"</code>\
  \ </p> </li> <li> <p> <code>\\\"Stop Reason RECYCLE_TASK\\\"</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"ReplicationTaskCreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"The date the replication task was created.\"\n        }\n      ]\n    },\n    \"ReplicationTaskStartDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"The date the replication task is scheduled to start.\"\n        }\n      ]\n    },\n    \"CdcStartPosition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>Indicates when you want a change data capture (CDC) operation to start. Use either <code>CdcStartPosition</code> or <code>CdcStartTime</code> to specify when you want the CDC operation to start. Specifying both\
  \ values results in an error.</p> <p>The value can be in date, checkpoint, or LSN/SCN format.</p> <p>Date Example: --cdc-start-position \\u201c2018-03-08T12:12:12\\u201d</p> <p>Checkpoint Example: --cdc-start-position \\\"checkpoint:V1#27#mysql-bin-changelog.157832:1975:-1:2002:677883278264080:mysql-bin-changelog.157832:1876#0#0#*#0#93\\\"</p> <p>LSN Example: --cdc-start-position \\u201cmysql-bin-changelog.000024:373\\u201d</p>\"\n        }\n      ]\n    },\n    \"CdcStopPosition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>Indicates when you want a change data capture (CDC) operation to stop. The value can be either server time or commit time.</p> <p>Server time example: --cdc-stop-position \\u201cserver_time:2018-02-09T12:12:12\\u201d</p> <p>Commit time example: --cdc-stop-position \\u201ccommit_time: 2018-02-09T12:12:12\\u201c</p>\"\n        }\n      ]\n    },\n    \"RecoveryCheckpoint\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Indicates the last checkpoint that occurred during a change data capture (CDC) operation. You can provide this value to the <code>CdcStartPosition</code> parameter to start a CDC operation that begins at that checkpoint.\"\n        }\n      ]\n    },\n    \"ReplicationTaskArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the replication task.\"\n        }\n      ]\n    },\n    \"ReplicationTaskStats\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReplicationTaskStats\"\n        },\n        {\n          \"description\": \"The statistics for the task, including elapsed time, tables loaded, and table errors.\"\n        }\n      ]\n    },\n    \"TaskData\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Supplemental information that the task requires to migrate the data for certain source and target endpoints. For more information, see <a href=\\\"https://docs.aws.amazon.com/dms/latest/userguide/CHAP_Tasks.TaskData.html\\\">Specifying Supplemental Data for Task Settings</a> in the <i>Database Migration Service User Guide.</i> \"\n        }\n      ]\n    },\n    \"TargetReplicationInstanceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ARN of the replication instance to which this task is moved in response to running the <a href=\\\"https://docs.aws.amazon.com/dms/latest/APIReference/API_MoveReplicationTask.html\\\"> <code>MoveReplicationTask</code> </a> operation. Otherwise, this response parameter isn't a member of the <code>ReplicationTask</code> object.\"\n        }\n      ]\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-replication-task-schema.json
tags:
- Data Replication
- Database
- Database Migration
- Migration
title: ReplicationTask
---
