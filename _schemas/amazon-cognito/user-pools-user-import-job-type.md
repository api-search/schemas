---
description: The user import job type.
layout: schema
name: UserImportJobType
properties_list:
- description: ''
  name: JobName
  type: object
- description: ''
  name: JobId
  type: object
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: PreSignedUrl
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: StartDate
  type: object
- description: ''
  name: CompletionDate
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: CloudWatchLogsRoleArn
  type: object
- description: ''
  name: ImportedUsers
  type: object
- description: ''
  name: SkippedUsers
  type: object
- description: ''
  name: FailedUsers
  type: object
- description: ''
  name: CompletionMessage
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-user-import-job-type-schema.json
slug: user-pools-user-import-job-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-user-import-job-type-schema.json\",\n  \"title\": \"UserImportJobType\",\n  \"description\": \"The user import job type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserImportJobNameType\"\n        },\n        {\n          \"description\": \"The job name for the user import job.\"\n        }\n      ]\n    },\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserImportJobIdType\"\n        },\n        {\n          \"description\": \"The job ID for the user import job.\"\n        }\n      ]\n    },\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\"\
  : \"The user pool ID for the user pool that the users are being imported into.\"\n        }\n      ]\n    },\n    \"PreSignedUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PreSignedUrlType\"\n        },\n        {\n          \"description\": \"The pre-signed URL to be used to upload the <code>.csv</code> file.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date and time, in <a href=\\\"https://www.iso.org/iso-8601-date-and-time-format.html\\\">ISO 8601</a> format, when the item was created.\"\n        }\n      ]\n    },\n    \"StartDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date when the user import job was started.\"\n        }\n      ]\n    },\n    \"CompletionDate\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date when the user import job was completed.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserImportJobStatusType\"\n        },\n        {\n          \"description\": \"<p>The status of the user import job. One of the following:</p> <ul> <li> <p> <code>Created</code> - The job was created but not started.</p> </li> <li> <p> <code>Pending</code> - A transition state. You have started the job, but it has not begun importing users yet.</p> </li> <li> <p> <code>InProgress</code> - The job has started, and users are being imported.</p> </li> <li> <p> <code>Stopping</code> - You have stopped the job, but the job has not stopped importing users yet.</p> </li> <li> <p> <code>Stopped</code> - You have stopped the job, and the job has stopped importing users.</p> </li> <li> <p> <code>Succeeded</code>\
  \ - The job has completed successfully.</p> </li> <li> <p> <code>Failed</code> - The job has stopped due to an error.</p> </li> <li> <p> <code>Expired</code> - You created a job, but did not start the job within 24-48 hours. All data associated with the job was deleted, and the job can't be started.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"CloudWatchLogsRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"The role Amazon Resource Name (ARN) for the Amazon CloudWatch Logging role for the user import job. For more information, see \\\"Creating the CloudWatch Logs IAM Role\\\" in the Amazon Cognito Developer Guide.\"\n        }\n      ]\n    },\n    \"ImportedUsers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongType\"\n        },\n        {\n          \"description\": \"The number of users that were successfully imported.\"\n        }\n      ]\n\
  \    },\n    \"SkippedUsers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongType\"\n        },\n        {\n          \"description\": \"The number of users that were skipped.\"\n        }\n      ]\n    },\n    \"FailedUsers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongType\"\n        },\n        {\n          \"description\": \"The number of users that couldn't be imported.\"\n        }\n      ]\n    },\n    \"CompletionMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CompletionMessageType\"\n        },\n        {\n          \"description\": \"The message returned when the user import job is completed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-user-import-job-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: UserImportJobType
---
