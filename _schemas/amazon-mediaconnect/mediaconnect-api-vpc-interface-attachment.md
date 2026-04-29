---
description: The settings for attaching a VPC interface to an resource.
layout: schema
name: VpcInterfaceAttachment
properties_list:
- description: ''
  name: VpcInterfaceName
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-vpc-interface-attachment-schema.json
slug: mediaconnect-api-vpc-interface-attachment
source_filename: mediaconnect-api-vpc-interface-attachment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-vpc-interface-attachment-schema.json\",\n  \"title\": \"VpcInterfaceAttachment\",\n  \"description\": \"The settings for attaching a VPC interface to an resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcInterfaceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vpcInterfaceName\"\n          },\n          \"description\": \"The name of the VPC interface to use for this resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-vpc-interface-attachment-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: VpcInterfaceAttachment
---
