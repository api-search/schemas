---
description: CreateCrawlerRequest schema from Amazon Glue API
layout: schema
name: CreateCrawlerRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Role
  type: object
- description: ''
  name: DatabaseName
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Targets
  type: object
- description: ''
  name: Schedule
  type: object
- description: ''
  name: Classifiers
  type: object
- description: ''
  name: TablePrefix
  type: object
- description: ''
  name: SchemaChangePolicy
  type: object
- description: ''
  name: RecrawlPolicy
  type: object
- description: ''
  name: LineageConfiguration
  type: object
- description: ''
  name: LakeFormationConfiguration
  type: object
- description: ''
  name: Configuration
  type: object
- description: ''
  name: CrawlerSecurityConfiguration
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-create-crawler-request-schema.json
slug: glue-create-crawler-request
source_filename: glue-create-crawler-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-crawler-request-schema.json\",\n  \"title\": \"CreateCrawlerRequest\",\n  \"description\": \"CreateCrawlerRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"Name of the new crawler.\"\n        }\n      ]\n    },\n    \"Role\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Role\"\n        },\n        {\n          \"description\": \"The IAM role or Amazon Resource Name (ARN) of an IAM role used by the new crawler to access customer resources.\"\n        }\n      ]\n    },\n    \"DatabaseName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatabaseName\"\
  \n        },\n        {\n          \"description\": \"The Glue database where results are written, such as: <code>arn:aws:daylight:us-east-1::database/sometable/*</code>.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescriptionString\"\n        },\n        {\n          \"description\": \"A description of the new crawler.\"\n        }\n      ]\n    },\n    \"Targets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CrawlerTargets\"\n        },\n        {\n          \"description\": \"A list of collection of targets to crawl.\"\n        }\n      ]\n    },\n    \"Schedule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CronExpression\"\n        },\n        {\n          \"description\": \"A <code>cron</code> expression used to specify the schedule (see <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/monitor-data-warehouse-schedule.html\\\"\
  >Time-Based Schedules for Jobs and Crawlers</a>. For example, to run something every day at 12:15 UTC, you would specify: <code>cron(15 12 * * ? *)</code>.\"\n        }\n      ]\n    },\n    \"Classifiers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClassifierNameList\"\n        },\n        {\n          \"description\": \"A list of custom classifiers that the user has registered. By default, all built-in classifiers are included in a crawl, but these custom classifiers always override the default classifiers for a given classification.\"\n        }\n      ]\n    },\n    \"TablePrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TablePrefix\"\n        },\n        {\n          \"description\": \"The table prefix used for catalog tables that are created.\"\n        }\n      ]\n    },\n    \"SchemaChangePolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaChangePolicy\"\n        },\n\
  \        {\n          \"description\": \"The policy for the crawler's update and deletion behavior.\"\n        }\n      ]\n    },\n    \"RecrawlPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecrawlPolicy\"\n        },\n        {\n          \"description\": \"A policy that specifies whether to crawl the entire dataset again, or to crawl only folders that were added since the last crawler run.\"\n        }\n      ]\n    },\n    \"LineageConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LineageConfiguration\"\n        },\n        {\n          \"description\": \"Specifies data lineage configuration settings for the crawler.\"\n        }\n      ]\n    },\n    \"LakeFormationConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LakeFormationConfiguration\"\n        },\n        {\n          \"description\": \"Specifies Lake Formation configuration settings for the crawler.\"\
  \n        }\n      ]\n    },\n    \"Configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CrawlerConfiguration\"\n        },\n        {\n          \"description\": \"Crawler configuration information. This versioned JSON string allows users to specify aspects of a crawler's behavior. For more information, see <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/crawler-configuration.html\\\">Setting crawler configuration options</a>.\"\n        }\n      ]\n    },\n    \"CrawlerSecurityConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CrawlerSecurityConfiguration\"\n        },\n        {\n          \"description\": \"The name of the <code>SecurityConfiguration</code> structure to be used by this crawler.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"The tags to use\
  \ with this crawler request. You may use tags to limit access to the crawler. For more information about tags in Glue, see <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/monitor-tags.html\\\">Amazon Web Services Tags in Glue</a> in the developer guide.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Role\",\n    \"Targets\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-crawler-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreateCrawlerRequest
---
