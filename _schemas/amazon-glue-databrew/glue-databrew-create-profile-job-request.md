---
description: CreateProfileJobRequest schema from Amazon Glue DataBrew API
layout: schema
name: CreateProfileJobRequest
properties_list:
- description: ''
  name: DatasetName
  type: object
- description: ''
  name: EncryptionKeyArn
  type: object
- description: ''
  name: EncryptionMode
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: LogSubscription
  type: object
- description: ''
  name: MaxCapacity
  type: object
- description: ''
  name: MaxRetries
  type: object
- description: ''
  name: OutputLocation
  type: object
- description: ''
  name: Configuration
  type: object
- description: ''
  name: ValidationConfigurations
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: Timeout
  type: object
- description: ''
  name: JobSample
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-create-profile-job-request-schema.json
slug: glue-databrew-create-profile-job-request
source_filename: glue-databrew-create-profile-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-create-profile-job-request-schema.json\",\n  \"title\": \"CreateProfileJobRequest\",\n  \"description\": \"CreateProfileJobRequest schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatasetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetName\"\n        },\n        {\n          \"description\": \"The name of the dataset that this job is to act upon.\"\n        }\n      ]\n    },\n    \"EncryptionKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionKeyArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of an encryption key that is used to protect the job.\"\n        }\n      ]\n    },\n    \"EncryptionMode\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionMode\"\n        },\n        {\n          \"description\": \"<p>The encryption mode for the job, which can be one of the following:</p> <ul> <li> <p> <code>SSE-KMS</code> - <code>SSE-KMS</code> - Server-side encryption with KMS-managed keys.</p> </li> <li> <p> <code>SSE-S3</code> - Server-side encryption with keys managed by Amazon S3.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobName\"\n        },\n        {\n          \"description\": \"The name of the job to be created. Valid characters are alphanumeric (A-Z, a-z, 0-9), hyphen (-), period (.), and space.\"\n        }\n      ]\n    },\n    \"LogSubscription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogSubscription\"\n        },\n        {\n          \"description\": \"Enables or disables Amazon CloudWatch logging for the job. If\
  \ logging is enabled, CloudWatch writes one log stream for each job run.\"\n        }\n      ]\n    },\n    \"MaxCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxCapacity\"\n        },\n        {\n          \"description\": \"The maximum number of nodes that DataBrew can use when the job processes data.\"\n        }\n      ]\n    },\n    \"MaxRetries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxRetries\"\n        },\n        {\n          \"description\": \"The maximum number of times to retry the job after a job run fails.\"\n        }\n      ]\n    },\n    \"OutputLocation\": {\n      \"$ref\": \"#/components/schemas/S3Location\"\n    },\n    \"Configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileConfiguration\"\n        },\n        {\n          \"description\": \"Configuration for profile jobs. Used to select columns, do evaluations, and override default parameters\
  \ of evaluations. When configuration is null, the profile job will run with default settings.\"\n        }\n      ]\n    },\n    \"ValidationConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValidationConfigurationList\"\n        },\n        {\n          \"description\": \"List of validation configurations that are applied to the profile job.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Identity and Access Management (IAM) role to be assumed when DataBrew runs the job.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Metadata tags to apply to this job.\"\n        }\n      ]\n    },\n    \"Timeout\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/Timeout\"\n        },\n        {\n          \"description\": \"The job's timeout in minutes. A job that attempts to run longer than this timeout period ends with a status of <code>TIMEOUT</code>.\"\n        }\n      ]\n    },\n    \"JobSample\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobSample\"\n        },\n        {\n          \"description\": \"Sample configuration for profile jobs only. Determines the number of rows on which the profile job will be executed. If a JobSample value is not provided, the default value will be used. The default value is CUSTOM_ROWS for the mode parameter and 20000 for the size parameter.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DatasetName\",\n    \"Name\",\n    \"OutputLocation\",\n    \"RoleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-create-profile-job-request-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: CreateProfileJobRequest
---
