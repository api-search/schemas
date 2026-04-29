---
description: A collection of Amazon Web Services tags. Tags help you identify and organize your Amazon Web Services resources. Many Amazon Web Services services support tagging, so you can assign the same tag to resources from different services to indicate that the resources are related. For example, you can as
layout: schema
name: TagCollection
properties_list:
- description: ''
  name: AppBoundaryKey
  type: object
- description: ''
  name: TagValues
  type: object
provider_name: Amazon DevOps Guru
provider_slug: amazon-devops-guru
schema_file: json-schema/amazon-devops-guru-tag-collection-schema.json
slug: amazon-devops-guru-tag-collection
source_filename: amazon-devops-guru-tag-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-tag-collection-schema.json\",\n  \"title\": \"TagCollection\",\n  \"description\": \"A collection of Amazon Web Services tags. Tags help you identify and organize your Amazon Web Services resources. Many Amazon Web Services services support tagging, so you can assign the same tag to resources from different services to indicate that the resources are related. For example, you can as\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AppBoundaryKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AppBoundaryKey\"\n        },\n        {\n          \"description\": \"<p>An Amazon Web Services tag <i>key</i> that is used to identify the Amazon Web Services resources that DevOps Guru analyzes. All Amazon Web Services resources in your account and Region\
  \ tagged with this <i>key</i> make up your DevOps Guru application and analysis boundary.</p> <important> <p>The string used for a <i>key</i> in a tag that you use to define your resource coverage must begin with the prefix <code>Devops-guru-</code>. The tag <i>key</i> might be <code>DevOps-Guru-deployment-application</code> or <code>devops-guru-rds-application</code>. When you create a <i>key</i>, the case of characters in the <i>key</i> can be whatever you choose. After you create a <i>key</i>, it is case-sensitive. For example, DevOps Guru works with a <i>key</i> named <code>devops-guru-rds</code> and a <i>key</i> named <code>DevOps-Guru-RDS</code>, and these act as two different <i>keys</i>. Possible <i>key</i>/<i>value</i> pairs in your application might be <code>Devops-Guru-production-application/RDS</code> or <code>Devops-Guru-production-application/containers</code>.</p> </important>\"\n        }\n      ]\n    },\n    \"TagValues\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/TagValues\"\n        },\n        {\n          \"description\": \"<p>The values in an Amazon Web Services tag collection.</p> <p>The tag's <i>value</i> is an optional field used to associate a string with the tag <i>key</i> (for example, <code>111122223333</code>, <code>Production</code>, or a team name). The <i>key</i> and <i>value</i> are the tag's <i>key</i> pair. Omitting the tag <i>value</i> is the same as using an empty string. Like tag <i>keys</i>, tag <i>values</i> are case-sensitive. You can specify a maximum of 256 characters for a tag value.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AppBoundaryKey\",\n    \"TagValues\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-tag-collection-schema.json
tags:
- Anomaly Detection
- AWS
- DevOps
- Machine Learning
- Operational Intelligence
title: TagCollection
---
