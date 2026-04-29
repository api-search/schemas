---
description: DescribeClassificationJobResponse schema from Amazon Macie API
layout: schema
name: DescribeClassificationJobResponse
properties_list:
- description: ''
  name: allowListIds
  type: object
- description: ''
  name: clientToken
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: customDataIdentifierIds
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: initialRun
  type: object
- description: ''
  name: jobArn
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
  name: lastRunTime
  type: object
- description: ''
  name: managedDataIdentifierIds
  type: object
- description: ''
  name: managedDataIdentifierSelector
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: s3JobDefinition
  type: object
- description: ''
  name: samplingPercentage
  type: object
- description: ''
  name: scheduleFrequency
  type: object
- description: ''
  name: statistics
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: userPausedDetails
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-describe-classification-job-response-schema.json
slug: amazon-macie-describe-classification-job-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-describe-classification-job-response-schema.json\",\n  \"title\": \"DescribeClassificationJobResponse\",\n  \"description\": \"DescribeClassificationJobResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowListIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"An array of unique identifiers, one for each allow list that the job uses when it analyzes data.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The token that was provided to ensure the idempotency of the request to create the job.\"\n        }\n\
  \      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when the job was created.\"\n        }\n      ]\n    },\n    \"customDataIdentifierIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"An array of unique identifiers, one for each custom data identifier that the job uses when it analyzes data. This value is null if the job uses only managed data identifiers to analyze data.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The custom description of the job.\"\n        }\n      ]\n    },\n    \"initialRun\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"For a recurring job, specifies whether you configured the job to analyze all existing, eligible objects immediately after the job was created (true). If you configured the job to analyze only those objects that were created or changed after the job was created and before the job's first scheduled run, this value is false. This value is also false for a one-time job.\"\n        }\n      ]\n    },\n    \"jobArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the job.\"\n        }\n      ]\n    },\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the job.\"\n        }\n      ]\n    },\n    \"jobStatus\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\": \"<p>The current status of the job. Possible values are:</p> <ul><li><p>CANCELLED - You cancelled the job or, if it's a one-time job, you paused the job and didn't resume it within 30 days.</p></li> <li><p>COMPLETE - For a one-time job, Amazon Macie finished processing the data specified for the job. This value doesn't apply to recurring jobs.</p></li> <li><p>IDLE - For a recurring job, the previous scheduled run is complete and the next scheduled run is pending. This value doesn't apply to one-time jobs.</p></li> <li><p>PAUSED - Macie started running the job but additional processing would exceed the monthly sensitive data discovery quota for your account or one or more member accounts that the job analyzes data for.</p></li> <li><p>RUNNING - For a one-time job, the job is in progress. For a recurring job, a scheduled run is in progress.</p></li> <li><p>USER_PAUSED - You paused the\
  \ job. If you paused the job while it had a status of RUNNING and you don't resume it within 30 days of pausing it, the job or job run will expire and be cancelled, depending on the job's type. To check the expiration date, refer to the UserPausedDetails.jobExpiresAt property.</p></li></ul>\"\n        }\n      ]\n    },\n    \"jobType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobType\"\n        },\n        {\n          \"description\": \"<p>The schedule for running the job. Possible values are:</p> <ul><li><p>ONE_TIME - The job runs only once.</p></li> <li><p>SCHEDULED - The job runs on a daily, weekly, or monthly basis. The scheduleFrequency property indicates the recurrence pattern for the job.</p></li></ul>\"\n        }\n      ]\n    },\n    \"lastRunErrorStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastRunErrorStatus\"\n        },\n        {\n          \"description\": \"Specifies whether any account- or\
  \ bucket-level access errors occurred when the job ran. For a recurring job, this value indicates the error status of the job's most recent run.\"\n        }\n      ]\n    },\n    \"lastRunTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when the job started. If the job is a recurring job, this value indicates when the most recent run started or, if the job hasn't run yet, when the job was created.\"\n        }\n      ]\n    },\n    \"managedDataIdentifierIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"An array of unique identifiers, one for each managed data identifier that the job is explicitly configured to include (use) or exclude (not use) when it analyzes data. Inclusion or exclusion depends on the managed data\
  \ identifier selection type specified for the job (managedDataIdentifierSelector). This value is null if the job's managed data identifier selection type is ALL or the job uses only custom data identifiers (customDataIdentifierIds) to analyze data.\"\n        }\n      ]\n    },\n    \"managedDataIdentifierSelector\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ManagedDataIdentifierSelector\"\n        },\n        {\n          \"description\": \"<p>The selection type that determines which managed data identifiers the job uses to analyze data. Possible values are:</p> <ul><li><p>ALL - Use all the managed data identifiers that Amazon Macie provides.</p></li> <li><p>EXCLUDE - Use all the managed data identifiers that Macie provides except the managed data identifiers specified by the managedDataIdentifierIds property.</p></li> <li><p>INCLUDE - Use only the managed data identifiers specified by the managedDataIdentifierIds property.</p></li> <li><p>NONE - Don't\
  \ use any managed data identifiers.</p></li></ul> <p>If this value is null, the job uses all managed data identifiers. If this value is null, ALL, or EXCLUDE for a recurring job, the job also uses new managed data identifiers as they are released.</p>\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The custom name of the job.\"\n        }\n      ]\n    },\n    \"s3JobDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3JobDefinition\"\n        },\n        {\n          \"description\": \"The S3 buckets that contain the objects to analyze, and the scope of that analysis.\"\n        }\n      ]\n    },\n    \"samplingPercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The sampling depth, as a percentage, that determines\
  \ the percentage of eligible objects that the job analyzes.\"\n        }\n      ]\n    },\n    \"scheduleFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobScheduleFrequency\"\n        },\n        {\n          \"description\": \"The recurrence pattern for running the job. This value is null if the job is configured to run only once.\"\n        }\n      ]\n    },\n    \"statistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Statistics\"\n        },\n        {\n          \"description\": \"The number of times that the job has run and processing statistics for the job's current run.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A map of key-value pairs that specifies which tags (keys and values) are associated with the classification job.\"\n        }\n      ]\n    },\n    \"\
  userPausedDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPausedDetails\"\n        },\n        {\n          \"description\": \"If the current status of the job is USER_PAUSED, specifies when the job was paused and when the job or job run will expire and be cancelled if it isn't resumed. This value is present only if the value for jobStatus is USER_PAUSED.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-describe-classification-job-response-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: DescribeClassificationJobResponse
---
