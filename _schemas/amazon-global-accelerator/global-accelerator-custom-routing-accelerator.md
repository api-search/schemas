---
description: Attributes of a custom routing accelerator.
layout: schema
name: CustomRoutingAccelerator
properties_list:
- description: ''
  name: AcceleratorArn
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: IpAddressType
  type: object
- description: ''
  name: Enabled
  type: object
- description: ''
  name: IpSets
  type: object
- description: ''
  name: DnsName
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: CreatedTime
  type: object
- description: ''
  name: LastModifiedTime
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-custom-routing-accelerator-schema.json
slug: global-accelerator-custom-routing-accelerator
source_filename: global-accelerator-custom-routing-accelerator-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-custom-routing-accelerator-schema.json\",\n  \"title\": \"CustomRoutingAccelerator\",\n  \"description\": \"Attributes of a custom routing accelerator.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AcceleratorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the custom routing accelerator.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The name of the accelerator. The name must contain only alphanumeric characters or hyphens (-), and must not begin or end with a hyphen.\"\n        }\n   \
  \   ]\n    },\n    \"IpAddressType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddressType\"\n        },\n        {\n          \"description\": \"The IP address type that an accelerator supports. For a custom routing accelerator, the value must be IPV4.\"\n        }\n      ]\n    },\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericBoolean\"\n        },\n        {\n          \"description\": \"<p>Indicates whether the accelerator is enabled. The value is true or false. The default value is true. </p> <p>If the value is set to true, the accelerator cannot be deleted. If set to false, accelerator can be deleted.</p>\"\n        }\n      ]\n    },\n    \"IpSets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpSets\"\n        },\n        {\n          \"description\": \"The static IP addresses that Global Accelerator associates with the accelerator.\"\n        }\n      ]\n\
  \    },\n    \"DnsName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"<p>The Domain Name System (DNS) name that Global Accelerator creates that points to an accelerator's static IPv4 addresses. </p> <p>The naming convention for the DNS name is the following: A lowercase letter a, followed by a 16-bit random hex string, followed by .awsglobalaccelerator.com. For example: a1234567890abcdef.awsglobalaccelerator.com.</p> <p>If you have a dual-stack accelerator, you also have a second DNS name, <code>DualStackDnsName</code>, that points to both the A record and the AAAA record for all four static addresses for the accelerator: two IPv4 addresses and two IPv6 addresses.</p> <p>For more information about the default DNS name, see <a href=\\\"https://docs.aws.amazon.com/global-accelerator/latest/dg/dns-addressing-custom-domains.dns-addressing.html\\\"> Support for DNS addressing in Global Accelerator</a>\
  \ in the <i>Global Accelerator Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomRoutingAcceleratorStatus\"\n        },\n        {\n          \"description\": \"Describes the deployment status of the accelerator.\"\n        }\n      ]\n    },\n    \"CreatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time that the accelerator was created.\"\n        }\n      ]\n    },\n    \"LastModifiedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time that the accelerator was last modified.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-custom-routing-accelerator-schema.json
tags:
- Availability
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: CustomRoutingAccelerator
---
