---
description: The metadata options for the instances. For more information, see <a href="https://docs.aws.amazon.com/autoscaling/ec2/userguide/create-launch-config.html#launch-configurations-imds">Configuring the Instance Metadata Options</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.
layout: schema
name: InstanceMetadataOptions
properties_list:
- description: ''
  name: HttpTokens
  type: object
- description: ''
  name: HttpPutResponseHopLimit
  type: object
- description: ''
  name: HttpEndpoint
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-instance-metadata-options-schema.json
slug: ec2-auto-scaling-instance-metadata-options
source_filename: ec2-auto-scaling-instance-metadata-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-instance-metadata-options-schema.json\",\n  \"title\": \"InstanceMetadataOptions\",\n  \"description\": \"The metadata options for the instances. For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/create-launch-config.html#launch-configurations-imds\\\">Configuring the Instance Metadata Options</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HttpTokens\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceMetadataHttpTokensState\"\n        },\n        {\n          \"description\": \"<p>The state of token usage for your instance metadata requests. If the parameter is not specified in the request, the default state is <code>optional</code>.</p>\
  \ <p>If the state is <code>optional</code>, you can choose to retrieve instance metadata with or without a signed token header on your request. If you retrieve the IAM role credentials without a token, the version 1.0 role credentials are returned. If you retrieve the IAM role credentials using a valid signed token, the version 2.0 role credentials are returned.</p> <p>If the state is <code>required</code>, you must send a signed token header with any instance metadata retrieval requests. In this state, retrieving the IAM role credentials always returns the version 2.0 credentials; the version 1.0 credentials are not available.</p>\"\n        }\n      ]\n    },\n    \"HttpPutResponseHopLimit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceMetadataHttpPutResponseHopLimit\"\n        },\n        {\n          \"description\": \"<p>The desired HTTP PUT response hop limit for instance metadata requests. The larger the number, the further instance metadata\
  \ requests can travel.</p> <p>Default: 1</p>\"\n        }\n      ]\n    },\n    \"HttpEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceMetadataEndpointState\"\n        },\n        {\n          \"description\": \"<p>This parameter enables or disables the HTTP metadata endpoint on your instances. If the parameter is not specified, the default state is <code>enabled</code>.</p> <note> <p>If you specify a value of <code>disabled</code>, you will not be able to access your instance metadata. </p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-instance-metadata-options-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: InstanceMetadataOptions
---
