---
description: Provides information about a classification job, including the current status of the job.
layout: schema
name: JobSummary
properties_list:
- description: ''
  name: bucketCriteria
  type: object
- description: ''
  name: bucketDefinitions
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: jobId
  type: object
- description: ''
  name: jobStatus
  type: object
- description: ''
  name: jobType
  type: object
- description: ''
  name: lastRunErrorStatus
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: userPausedDetails
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-job-summary-schema.json
slug: amazon-macie-job-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-job-summary-schema.json\",\n  \"title\": \"JobSummary\",\n  \"description\": \"Provides information about a classification job, including the current status of the job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketCriteriaForJob\"\n        },\n        {\n          \"description\": \"The property- and tag-based conditions that determine which S3 buckets are included or excluded from the job's analysis. Each time the job runs, the job uses these criteria to determine which buckets to analyze. A job's definition can contain a bucketCriteria object or a bucketDefinitions array, not both.\"\n        }\n      ]\n    },\n    \"bucketDefinitions\": {\n      \"allOf\": [\n        {\n     \
  \     \"$ref\": \"#/components/schemas/__listOfS3BucketDefinitionForJob\"\n        },\n        {\n          \"description\": \"An array of objects, one for each Amazon Web Services account that owns specific S3 buckets for the job to analyze. Each object specifies the account ID for an account and one or more buckets to analyze for that account. A job's definition can contain a bucketDefinitions array or a bucketCriteria object, not both.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when the job was created.\"\n        }\n      ]\n    },\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the job.\"\n        }\n      ]\n    },\n    \"jobStatus\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\": \"<p>The current status of the job. Possible values are:</p> <ul><li><p>CANCELLED - You cancelled the job or, if it's a one-time job, you paused the job and didn't resume it within 30 days.</p></li> <li><p>COMPLETE - For a one-time job, Amazon Macie finished processing the data specified for the job. This value doesn't apply to recurring jobs.</p></li> <li><p>IDLE - For a recurring job, the previous scheduled run is complete and the next scheduled run is pending. This value doesn't apply to one-time jobs.</p></li> <li><p>PAUSED - Macie started running the job but additional processing would exceed the monthly sensitive data discovery quota for your account or one or more member accounts that the job analyzes data for.</p></li> <li><p>RUNNING - For a one-time job, the job is in progress. For a recurring job, a scheduled run is in progress.</p></li> <li><p>USER_PAUSED\
  \ - You paused the job. If you paused the job while it had a status of RUNNING and you don't resume it within 30 days of pausing it, the job or job run will expire and be cancelled, depending on the job's type. To check the expiration date, refer to the UserPausedDetails.jobExpiresAt property.</p></li></ul>\"\n        }\n      ]\n    },\n    \"jobType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobType\"\n        },\n        {\n          \"description\": \"<p>The schedule for running the job. Possible values are:</p> <ul><li><p>ONE_TIME - The job runs only once.</p></li> <li><p>SCHEDULED - The job runs on a daily, weekly, or monthly basis.</p></li></ul>\"\n        }\n      ]\n    },\n    \"lastRunErrorStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastRunErrorStatus\"\n        },\n        {\n          \"description\": \"Specifies whether any account- or bucket-level access errors occurred when the job ran. For\
  \ a recurring job, this value indicates the error status of the job's most recent run.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The custom name of the job.\"\n        }\n      ]\n    },\n    \"userPausedDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPausedDetails\"\n        },\n        {\n          \"description\": \"If the current status of the job is USER_PAUSED, specifies when the job was paused and when the job or job run will expire and be cancelled if it isn't resumed. This value is present only if the value for jobStatus is USER_PAUSED.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-job-summary-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: JobSummary
---
