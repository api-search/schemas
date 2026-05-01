---
description: The instance metadata options that apply to the HTTP requests that pipeline builds use to launch EC2 build and test instances. For more information about instance metadata options, see <a href="https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/configuring-instance-metadata-options.html">Configure the instance metadata options</a> in the <i> <i>Amazon EC2 User Guide</i> </i> for Linux instances, or <a href="https://docs.aws.amazon.com/AWSEC2/latest/WindowsGuide/configuring-instance-metadata-options.html">Configure the instance metadata options</a> in the <i> <i>Amazon EC2 Windows Guide</i> </i> for Windows instances.
layout: schema
name: InstanceMetadataOptions
properties_list:
- description: ''
  name: httpTokens
  type: object
- description: ''
  name: httpPutResponseHopLimit
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-instance-metadata-options-schema.json
slug: ec2-image-builder-instance-metadata-options
source_filename: ec2-image-builder-instance-metadata-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-instance-metadata-options-schema.json\",\n  \"title\": \"InstanceMetadataOptions\",\n  \"description\": \"The instance metadata options that apply to the HTTP requests that pipeline builds use to launch EC2 build and test instances. For more information about instance metadata options, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/configuring-instance-metadata-options.html\\\">Configure the instance metadata options</a> in the <i> <i>Amazon EC2 User Guide</i> </i> for Linux instances, or <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/WindowsGuide/configuring-instance-metadata-options.html\\\">Configure the instance metadata options</a> in the <i> <i>Amazon EC2 Windows Guide</i> </i> for Windows instances.\",\n  \"type\": \"object\",\n  \"properties\"\
  : {\n    \"httpTokens\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpTokens\"\n        },\n        {\n          \"description\": \"<p>Indicates whether a signed token header is required for instance metadata retrieval requests. The values affect the response as follows:</p> <ul> <li> <p> <b>required</b> \\u2013 When you retrieve the IAM role credentials, version 2.0 credentials are returned in all cases.</p> </li> <li> <p> <b>optional</b> \\u2013 You can include a signed token header in your request to retrieve instance metadata, or you can leave it out. If you include it, version 2.0 credentials are returned for the IAM role. Otherwise, version 1.0 credentials are returned.</p> </li> </ul> <p>The default setting is <b>optional</b>.</p>\"\n        }\n      ]\n    },\n    \"httpPutResponseHopLimit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpPutResponseHopLimit\"\n        },\n        {\n          \"description\"\
  : \"Limit the number of hops that an instance metadata request can traverse to reach its destination. The default is one hop. However, if HTTP tokens are required, container image builds need a minimum of two hops.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-instance-metadata-options-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: InstanceMetadataOptions
---
