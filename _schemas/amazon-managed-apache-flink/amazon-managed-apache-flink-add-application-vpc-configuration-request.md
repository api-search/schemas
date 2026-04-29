---
description: AddApplicationVpcConfigurationRequest schema from Amazon Managed Service for Apache Flink API
layout: schema
name: AddApplicationVpcConfigurationRequest
properties_list:
- description: ''
  name: ApplicationName
  type: object
- description: ''
  name: CurrentApplicationVersionId
  type: object
- description: ''
  name: VpcConfiguration
  type: object
- description: ''
  name: ConditionalToken
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-add-application-vpc-configuration-request-schema.json
slug: amazon-managed-apache-flink-add-application-vpc-configuration-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-add-application-vpc-configuration-request-schema.json\",\n  \"title\": \"AddApplicationVpcConfigurationRequest\",\n  \"description\": \"AddApplicationVpcConfigurationRequest schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of an existing application.\"\n        }\n      ]\n    },\n    \"CurrentApplicationVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionId\"\n        },\n        {\n          \"description\": \"The version of the application to which you want to add the VPC\
  \ configuration. You must provide the <code>CurrentApplicationVersionId</code> or the <code>ConditionalToken</code>. You can use the <a>DescribeApplication</a> operation to get the current application version. If the version specified is not the current version, the <code>ConcurrentModificationException</code> is returned. For better concurrency support, use the <code>ConditionalToken</code> parameter instead of <code>CurrentApplicationVersionId</code>.\"\n        }\n      ]\n    },\n    \"VpcConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcConfiguration\"\n        },\n        {\n          \"description\": \"Description of the VPC to add to the application.\"\n        }\n      ]\n    },\n    \"ConditionalToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConditionalToken\"\n        },\n        {\n          \"description\": \"A value you use to implement strong concurrency for application updates. You must\
  \ provide the <code>ApplicationVersionID</code> or the <code>ConditionalToken</code>. You get the application's current <code>ConditionalToken</code> using <a>DescribeApplication</a>. For better concurrency support, use the <code>ConditionalToken</code> parameter instead of <code>CurrentApplicationVersionId</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationName\",\n    \"VpcConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-add-application-vpc-configuration-request-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: AddApplicationVpcConfigurationRequest
---
