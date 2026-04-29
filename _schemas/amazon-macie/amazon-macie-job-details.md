---
description: Specifies whether any one-time or recurring classification jobs are configured to analyze data in an S3 bucket, and, if so, the details of the job that ran most recently.
layout: schema
name: JobDetails
properties_list:
- description: ''
  name: isDefinedInJob
  type: object
- description: ''
  name: isMonitoredByJob
  type: object
- description: ''
  name: lastJobId
  type: object
- description: ''
  name: lastJobRunTime
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-job-details-schema.json
slug: amazon-macie-job-details
source_filename: amazon-macie-job-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-job-details-schema.json\",\n  \"title\": \"JobDetails\",\n  \"description\": \"Specifies whether any one-time or recurring classification jobs are configured to analyze data in an S3 bucket, and, if so, the details of the job that ran most recently.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"isDefinedInJob\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IsDefinedInJob\"\n        },\n        {\n          \"description\": \"<p>Specifies whether any one-time or recurring jobs are configured to analyze data in the bucket. Possible values are:</p> <ul><li><p>TRUE - The bucket is explicitly included in the bucket definition (S3BucketDefinitionForJob) for one or more jobs and at least one of those jobs has a status other than CANCELLED. Or the bucket matched\
  \ the bucket criteria (S3BucketCriteriaForJob) for at least one job that previously ran.</p></li> <li><p>FALSE - The bucket isn't explicitly included in the bucket definition (S3BucketDefinitionForJob) for any jobs, all the jobs that explicitly include the bucket in their bucket definitions have a status of CANCELLED, or the bucket didn't match the bucket criteria (S3BucketCriteriaForJob) for any jobs that previously ran.</p></li> <li><p>UNKNOWN - An exception occurred when Amazon Macie attempted to retrieve job data for the bucket.</p></li></ul>\"\n        }\n      ]\n    },\n    \"isMonitoredByJob\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IsMonitoredByJob\"\n        },\n        {\n          \"description\": \"<p>Specifies whether any recurring jobs are configured to analyze data in the bucket. Possible values are:</p> <ul><li><p>TRUE - The bucket is explicitly included in the bucket definition (S3BucketDefinitionForJob) for one or more recurring\
  \ jobs or the bucket matches the bucket criteria (S3BucketCriteriaForJob) for one or more recurring jobs. At least one of those jobs has a status other than CANCELLED.</p></li> <li><p>FALSE - The bucket isn't explicitly included in the bucket definition (S3BucketDefinitionForJob) for any recurring jobs, the bucket doesn't match the bucket criteria (S3BucketCriteriaForJob) for any recurring jobs, or all the recurring jobs that are configured to analyze data in the bucket have a status of CANCELLED.</p></li> <li><p>UNKNOWN - An exception occurred when Amazon Macie attempted to retrieve job data for the bucket.</p></li></ul>\"\n        }\n      ]\n    },\n    \"lastJobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"<p>The unique identifier for the job that ran most recently and is configured to analyze data in the bucket, either the latest run of a recurring job or the only run of a one-time\
  \ job.</p> <p>This value is typically null if the value for the isDefinedInJob property is FALSE or UNKNOWN.</p>\"\n        }\n      ]\n    },\n    \"lastJobRunTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"<p>The date and time, in UTC and extended ISO 8601 format, when the job (lastJobId) started. If the job is a recurring job, this value indicates when the most recent run started.</p> <p>This value is typically null if the value for the isDefinedInJob property is FALSE or UNKNOWN.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-job-details-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: JobDetails
---
