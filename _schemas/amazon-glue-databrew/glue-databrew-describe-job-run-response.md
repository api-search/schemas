---
description: DescribeJobRunResponse schema from Amazon Glue DataBrew API
layout: schema
name: DescribeJobRunResponse
properties_list:
- description: ''
  name: Attempt
  type: object
- description: ''
  name: CompletedOn
  type: object
- description: ''
  name: DatasetName
  type: object
- description: ''
  name: ErrorMessage
  type: object
- description: ''
  name: ExecutionTime
  type: object
- description: ''
  name: JobName
  type: object
- description: ''
  name: ProfileConfiguration
  type: object
- description: ''
  name: ValidationConfigurations
  type: object
- description: ''
  name: RunId
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: LogSubscription
  type: object
- description: ''
  name: LogGroupName
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
  name: RecipeReference
  type: object
- description: ''
  name: StartedBy
  type: object
- description: ''
  name: StartedOn
  type: object
- description: ''
  name: JobSample
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-describe-job-run-response-schema.json
slug: glue-databrew-describe-job-run-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-describe-job-run-response-schema.json\",\n  \"title\": \"DescribeJobRunResponse\",\n  \"description\": \"DescribeJobRunResponse schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Attempt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Attempt\"\n        },\n        {\n          \"description\": \"The number of times that DataBrew has attempted to run the job.\"\n        }\n      ]\n    },\n    \"CompletedOn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The date and time when the job completed processing.\"\n        }\n      ]\n    },\n    \"DatasetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetName\"\
  \n        },\n        {\n          \"description\": \"The name of the dataset for the job to process.\"\n        }\n      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobRunErrorMessage\"\n        },\n        {\n          \"description\": \"A message indicating an error (if any) that was encountered when the job ran.\"\n        }\n      ]\n    },\n    \"ExecutionTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionTime\"\n        },\n        {\n          \"description\": \"The amount of time, in seconds, during which the job run consumed resources.\"\n        }\n      ]\n    },\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobName\"\n        },\n        {\n          \"description\": \"The name of the job being processed during this run.\"\n        }\n      ]\n    },\n    \"ProfileConfiguration\": {\n      \"allOf\": [\n        {\n  \
  \        \"$ref\": \"#/components/schemas/ProfileConfiguration\"\n        },\n        {\n          \"description\": \"Configuration for profile jobs. Used to select columns, do evaluations, and override default parameters of evaluations. When configuration is null, the profile job will run with default settings.\"\n        }\n      ]\n    },\n    \"ValidationConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValidationConfigurationList\"\n        },\n        {\n          \"description\": \"List of validation configurations that are applied to the profile job.\"\n        }\n      ]\n    },\n    \"RunId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobRunId\"\n        },\n        {\n          \"description\": \"The unique identifier of the job run.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobRunState\"\n        },\n        {\n   \
  \       \"description\": \"The current state of the job run entity itself.\"\n        }\n      ]\n    },\n    \"LogSubscription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogSubscription\"\n        },\n        {\n          \"description\": \"The current status of Amazon CloudWatch logging for the job run.\"\n        }\n      ]\n    },\n    \"LogGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogGroupName\"\n        },\n        {\n          \"description\": \"The name of an Amazon CloudWatch log group, where the job writes diagnostic messages when it runs.\"\n        }\n      ]\n    },\n    \"Outputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputList\"\n        },\n        {\n          \"description\": \"One or more output artifacts from a job run.\"\n        }\n      ]\n    },\n    \"DataCatalogOutputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataCatalogOutputList\"\
  \n        },\n        {\n          \"description\": \"One or more artifacts that represent the Glue Data Catalog output from running the job.\"\n        }\n      ]\n    },\n    \"DatabaseOutputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatabaseOutputList\"\n        },\n        {\n          \"description\": \"Represents a list of JDBC database output objects which defines the output destination for a DataBrew recipe job to write into.\"\n        }\n      ]\n    },\n    \"RecipeReference\": {\n      \"$ref\": \"#/components/schemas/RecipeReference\"\n    },\n    \"StartedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StartedBy\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user who started the job run.\"\n        }\n      ]\n    },\n    \"StartedOn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"\
  description\": \"The date and time when the job run began.\"\n        }\n      ]\n    },\n    \"JobSample\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobSample\"\n        },\n        {\n          \"description\": \"Sample configuration for profile jobs only. Determines the number of rows on which the profile job will be executed. If a JobSample value is not provided, the default value will be used. The default value is CUSTOM_ROWS for the mode parameter and 20000 for the size parameter.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"JobName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-describe-job-run-response-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: DescribeJobRunResponse
---
