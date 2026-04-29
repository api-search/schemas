---
description: Describes a resume cluster operation. For example, a scheduled action to run the <code>ResumeCluster</code> API operation.
layout: schema
name: ResumeClusterMessage
properties_list:
- description: ''
  name: ClusterIdentifier
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-resume-cluster-message-schema.json
slug: redshift-resume-cluster-message
source_filename: redshift-resume-cluster-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {}\n  },\n  \"required\": [\n    \"ClusterIdentifier\"\n  ],\n  \"description\": \"Describes a resume cluster operation. For example, a scheduled action to run the <code>ResumeCluster</code> API operation. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-resume-cluster-message-schema.json\",\n  \"title\": \"ResumeClusterMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-resume-cluster-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ResumeClusterMessage
---
