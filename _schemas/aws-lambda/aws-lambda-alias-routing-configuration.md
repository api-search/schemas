---
description: The traffic-shifting configuration of a Lambda function alias. Used for weighted alias routing to enable canary deployments.
layout: schema
name: AliasRoutingConfiguration
properties_list:
- description: The secondary version weight. The key is the version number or alias name and the value is the percentage of traffic (0.0-1.0).
  name: AdditionalVersionWeights
  type: object
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-alias-routing-configuration-schema.json
slug: aws-lambda-alias-routing-configuration
source_filename: aws-lambda-alias-routing-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AliasRoutingConfiguration\",\n  \"type\": \"object\",\n  \"description\": \"The traffic-shifting configuration of a Lambda function alias. Used for weighted alias routing to enable canary deployments.\",\n  \"properties\": {\n    \"AdditionalVersionWeights\": {\n      \"type\": \"object\",\n      \"description\": \"The secondary version weight. The key is the version number or alias name and the value is the percentage of traffic (0.0-1.0).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-alias-routing-configuration-schema.json
tags: []
title: AliasRoutingConfiguration
---
