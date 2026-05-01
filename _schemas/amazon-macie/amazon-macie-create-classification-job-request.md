---
description: CreateClassificationJobRequest schema from Amazon Macie API
layout: schema
name: CreateClassificationJobRequest
properties_list:
- description: ''
  name: allowListIds
  type: object
- description: ''
  name: clientToken
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
  name: jobType
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
  name: tags
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-create-classification-job-request-schema.json
slug: amazon-macie-create-classification-job-request
source_filename: amazon-macie-create-classification-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-create-classification-job-request-schema.json\",\n  \"title\": \"CreateClassificationJobRequest\",\n  \"description\": \"CreateClassificationJobRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowListIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"An array of unique identifiers, one for each allow list for the job to use when it analyzes data.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A unique, case-sensitive token that you provide to ensure the idempotency of the request.\"\n        }\n     \
  \ ]\n    },\n    \"customDataIdentifierIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"An array of unique identifiers, one for each custom data identifier for the job to use when it analyzes data. To use only managed data identifiers, don't specify a value for this property and specify a value other than NONE for the managedDataIdentifierSelector property.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A custom description of the job. The description can contain as many as 200 characters.\"\n        }\n      ]\n    },\n    \"initialRun\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"<p>For a recurring job, specifies whether to analyze all existing,\
  \ eligible objects immediately after the job is created (true). To analyze only those objects that are created or changed after you create the job and before the job's first scheduled run, set this value to false.</p> <p>If you configure the job to run only once, don't specify a value for this property.</p>\"\n        }\n      ]\n    },\n    \"jobType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobType\"\n        },\n        {\n          \"description\": \"<p>The schedule for running the job. Valid values are:</p> <ul><li><p>ONE_TIME - Run the job only once. If you specify this value, don't specify a value for the scheduleFrequency property.</p></li> <li><p>SCHEDULED - Run the job on a daily, weekly, or monthly basis. If you specify this value, use the scheduleFrequency property to define the recurrence pattern for the job.</p></li></ul>\"\n        }\n      ]\n    },\n    \"managedDataIdentifierIds\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"<p>An array of unique identifiers, one for each managed data identifier for the job to include (use) or exclude (not use) when it analyzes data. Inclusion or exclusion depends on the managed data identifier selection type that you specify for the job (managedDataIdentifierSelector).</p> <p>To retrieve a list of valid values for this property, use the ListManagedDataIdentifiers operation.</p>\"\n        }\n      ]\n    },\n    \"managedDataIdentifierSelector\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ManagedDataIdentifierSelector\"\n        },\n        {\n          \"description\": \"<p>The selection type to apply when determining which managed data identifiers the job uses to analyze data. Valid values are:</p> <ul><li><p>ALL - Use all the managed data identifiers that Amazon Macie provides. If you specify this value, don't specify any values for the managedDataIdentifierIds\
  \ property.</p></li> <li><p>EXCLUDE - Use all the managed data identifiers that Macie provides except the managed data identifiers specified by the managedDataIdentifierIds property.</p></li> <li><p>INCLUDE - Use only the managed data identifiers specified by the managedDataIdentifierIds property.</p></li> <li><p>NONE - Don't use any managed data identifiers. If you specify this value, specify at least one custom data identifier for the job (customDataIdentifierIds) and don't specify any values for the managedDataIdentifierIds property.</p></li></ul> <p>If you don't specify a value for this property, the job uses all managed data identifiers. If you don't specify a value for this property or you specify ALL or EXCLUDE for a recurring job, the job also uses new managed data identifiers as they are released.</p>\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\"\
  : \"A custom name for the job. The name can contain as many as 500 characters.\"\n        }\n      ]\n    },\n    \"s3JobDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3JobDefinition\"\n        },\n        {\n          \"description\": \"The S3 buckets that contain the objects to analyze, and the scope of that analysis.\"\n        }\n      ]\n    },\n    \"samplingPercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The sampling depth, as a percentage, for the job to apply when processing objects. This value determines the percentage of eligible objects that the job analyzes. If this value is less than 100, Amazon Macie selects the objects to analyze at random, up to the specified percentage, and analyzes all the data in those objects.\"\n        }\n      ]\n    },\n    \"scheduleFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/JobScheduleFrequency\"\n        },\n        {\n          \"description\": \"The recurrence pattern for running the job. To run the job only once, don't specify a value for this property and set the value for the jobType property to ONE_TIME.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"<p>A map of key-value pairs that specifies the tags to associate with the job.</p> <p>A job can have a maximum of 50 tags. Each tag consists of a tag key and an associated tag value. The maximum length of a tag key is 128 characters. The maximum length of a tag value is 256 characters.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"s3JobDefinition\",\n    \"jobType\",\n    \"clientToken\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-create-classification-job-request-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: CreateClassificationJobRequest
---
