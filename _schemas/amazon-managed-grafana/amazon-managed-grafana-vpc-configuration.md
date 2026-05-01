---
description: <p>The configuration settings for an Amazon VPC that contains data sources for your Grafana workspace to connect to.</p> <note> <p>Provided <code>securityGroupIds</code> and <code>subnetIds</code> must be part of the same VPC.</p> <p>Connecting to a private VPC is not yet available in the Asia Pacific (Seoul) Region (ap-northeast-2).</p> </note>
layout: schema
name: VpcConfiguration
properties_list:
- description: ''
  name: securityGroupIds
  type: object
- description: ''
  name: subnetIds
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-vpc-configuration-schema.json
slug: amazon-managed-grafana-vpc-configuration
source_filename: amazon-managed-grafana-vpc-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-vpc-configuration-schema.json\",\n  \"title\": \"VpcConfiguration\",\n  \"description\": \"<p>The configuration settings for an Amazon VPC that contains data sources for your Grafana workspace to connect to.</p> <note> <p>Provided <code>securityGroupIds</code> and <code>subnetIds</code> must be part of the same VPC.</p> <p>Connecting to a private VPC is not yet available in the Asia Pacific (Seoul) Region (ap-northeast-2).</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"securityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroupIds\"\n        },\n        {\n          \"description\": \"The list of Amazon EC2 security group IDs attached to the Amazon VPC for your Grafana workspace to connect. Duplicates\
  \ not allowed.\"\n        }\n      ]\n    },\n    \"subnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetIds\"\n        },\n        {\n          \"description\": \"The list of Amazon EC2 subnet IDs created in the Amazon VPC for your Grafana workspace to connect. Duplicates not allowed.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"securityGroupIds\",\n    \"subnetIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-vpc-configuration-schema.json
tags:
- Dashboards
- Monitoring
- Observability
- Visualization
title: VpcConfiguration
---
