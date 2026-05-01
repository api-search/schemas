---
description: CreateAcceleratorRequest schema from Amazon Global Accelerator API
layout: schema
name: CreateAcceleratorRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: IpAddressType
  type: object
- description: ''
  name: IpAddresses
  type: object
- description: ''
  name: Enabled
  type: object
- description: ''
  name: IdempotencyToken
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-create-accelerator-request-schema.json
slug: global-accelerator-create-accelerator-request
source_filename: global-accelerator-create-accelerator-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-create-accelerator-request-schema.json\",\n  \"title\": \"CreateAcceleratorRequest\",\n  \"description\": \"CreateAcceleratorRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The name of the accelerator. The name can have a maximum of 64 characters, must contain only alphanumeric characters, periods (.), or hyphens (-), and must not begin or end with a hyphen or period.\"\n        }\n      ]\n    },\n    \"IpAddressType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddressType\"\n        },\n        {\n          \"description\": \"\
  The IP address type that an accelerator supports. For a standard accelerator, the value can be IPV4 or DUAL_STACK.\"\n        }\n      ]\n    },\n    \"IpAddresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddresses\"\n        },\n        {\n          \"description\": \"<p>Optionally, if you've added your own IP address pool to Global Accelerator (BYOIP), you can choose an IPv4 address from your own pool to use for the accelerator's static IPv4 address when you create an accelerator. </p> <p>After you bring an address range to Amazon Web Services, it appears in your account as an address pool. When you create an accelerator, you can assign one IPv4 address from your range to it. Global Accelerator assigns you a second static IPv4 address from an Amazon IP address range. If you bring two IPv4 address ranges to Amazon Web Services, you can assign one IPv4 address from each range to your accelerator. This restriction is because Global Accelerator assigns\
  \ each address range to a different network zone, for high availability.</p> <p>You can specify one or two addresses, separated by a space. Do not include the /32 suffix.</p> <p>Note that you can't update IP addresses for an existing accelerator. To change them, you must create a new accelerator with the new addresses.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/global-accelerator/latest/dg/using-byoip.html\\\">Bring your own IP addresses (BYOIP)</a> in the <i>Global Accelerator Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericBoolean\"\n        },\n        {\n          \"description\": \"<p>Indicates whether an accelerator is enabled. The value is true or false. The default value is true. </p> <p>If the value is set to true, an accelerator cannot be deleted. If set to false, the accelerator can be deleted.</p>\"\n        }\n      ]\n    },\n    \"IdempotencyToken\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdempotencyToken\"\n        },\n        {\n          \"description\": \"A unique, case-sensitive identifier that you provide to ensure the idempotency\\u2014that is, the uniqueness\\u2014of an accelerator.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"<p>Create tags for an accelerator.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/global-accelerator/latest/dg/tagging-in-global-accelerator.html\\\">Tagging in Global Accelerator</a> in the <i>Global Accelerator Developer Guide</i>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"IdempotencyToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-create-accelerator-request-schema.json
tags:
- Availability
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: CreateAcceleratorRequest
---
