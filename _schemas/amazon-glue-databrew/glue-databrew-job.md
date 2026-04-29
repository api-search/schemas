---
description: Represents all of the attributes of a DataBrew job.
layout: schema
name: Job
properties_list:
- description: ''
  name: AccountId
  type: object
- description: ''
  name: CreatedBy
  type: object
- description: ''
  name: CreateDate
  type: object
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
  name: Type
  type: object
- description: ''
  name: LastModifiedBy
  type: object
- description: ''
  name: LastModifiedDate
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
  name: Outputs
  type: object
- description: ''
  name: DataCatalogOutputs
  type: object
- description: ''
  name: DatabaseOutputs
  type: object
- description: ''
  name: ProjectName
  type: object
- description: ''
  name: RecipeReference
  type: object
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: Timeout
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: JobSample
  type: object
- description: ''
  name: ValidationConfigurations
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-job-schema.json
slug: glue-databrew-job
source_filename: glue-databrew-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-job-schema.json\",\n  \"title\": \"Job\",\n  \"description\": \"Represents all of the attributes of a DataBrew job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services account that owns the job.\"\n        }\n      ]\n    },\n    \"CreatedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedBy\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user who created the job.\"\n        }\n      ]\n    },\n    \"CreateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n \
  \       {\n          \"description\": \"The date and time that the job was created.\"\n        }\n      ]\n    },\n    \"DatasetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetName\"\n        },\n        {\n          \"description\": \"A dataset that the job is to process.\"\n        }\n      ]\n    },\n    \"EncryptionKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionKeyArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of an encryption key that is used to protect the job output. For more information, see <a href=\\\"https://docs.aws.amazon.com/databrew/latest/dg/encryption-security-configuration.html\\\">Encrypting data written by DataBrew jobs</a> \"\n        }\n      ]\n    },\n    \"EncryptionMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionMode\"\n        },\n        {\n          \"description\": \"<p>The encryption\
  \ mode for the job, which can be one of the following:</p> <ul> <li> <p> <code>SSE-KMS</code> - Server-side encryption with keys managed by KMS.</p> </li> <li> <p> <code>SSE-S3</code> - Server-side encryption with keys managed by Amazon S3.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobName\"\n        },\n        {\n          \"description\": \"The unique name of the job.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobType\"\n        },\n        {\n          \"description\": \"<p>The job type of the job, which must be one of the following:</p> <ul> <li> <p> <code>PROFILE</code> - A job to analyze a dataset, to determine its size, data types, data distribution, and more.</p> </li> <li> <p> <code>RECIPE</code> - A job to apply one or more transformations to a dataset.</p> </li> </ul>\"\n        }\n      ]\n    },\n  \
  \  \"LastModifiedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastModifiedBy\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user who last modified the job.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The modification date and time of the job.\"\n        }\n      ]\n    },\n    \"LogSubscription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogSubscription\"\n        },\n        {\n          \"description\": \"The current status of Amazon CloudWatch logging for the job.\"\n        }\n      ]\n    },\n    \"MaxCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxCapacity\"\n        },\n        {\n          \"description\": \"The maximum number of nodes that can be consumed when the job\
  \ processes data.\"\n        }\n      ]\n    },\n    \"MaxRetries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxRetries\"\n        },\n        {\n          \"description\": \"The maximum number of times to retry the job after a job run fails.\"\n        }\n      ]\n    },\n    \"Outputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputList\"\n        },\n        {\n          \"description\": \"One or more artifacts that represent output from running the job.\"\n        }\n      ]\n    },\n    \"DataCatalogOutputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataCatalogOutputList\"\n        },\n        {\n          \"description\": \"One or more artifacts that represent the Glue Data Catalog output from running the job.\"\n        }\n      ]\n    },\n    \"DatabaseOutputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatabaseOutputList\"\n      \
  \  },\n        {\n          \"description\": \"Represents a list of JDBC database output objects which defines the output destination for a DataBrew recipe job to write into.\"\n        }\n      ]\n    },\n    \"ProjectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectName\"\n        },\n        {\n          \"description\": \"The name of the project that the job is associated with.\"\n        }\n      ]\n    },\n    \"RecipeReference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeReference\"\n        },\n        {\n          \"description\": \"A set of steps that the job runs.\"\n        }\n      ]\n    },\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The unique Amazon Resource Name (ARN) for the job.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the role to be assumed for this job.\"\n        }\n      ]\n    },\n    \"Timeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timeout\"\n        },\n        {\n          \"description\": \"The job's timeout in minutes. A job that attempts to run longer than this timeout period ends with a status of <code>TIMEOUT</code>.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Metadata tags that have been applied to the job.\"\n        }\n      ]\n    },\n    \"JobSample\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobSample\"\n        },\n        {\n          \"description\": \"A sample configuration for profile jobs only, which determines the number of rows on which the\
  \ profile job is run. If a <code>JobSample</code> value isn't provided, the default value is used. The default value is CUSTOM_ROWS for the mode parameter and 20,000 for the size parameter.\"\n        }\n      ]\n    },\n    \"ValidationConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValidationConfigurationList\"\n        },\n        {\n          \"description\": \"List of validation configurations that are applied to the profile job.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-job-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: Job
---
