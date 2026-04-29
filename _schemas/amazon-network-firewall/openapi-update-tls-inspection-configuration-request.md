---
description: UpdateTLSInspectionConfigurationRequest schema from Amazon Network Firewall
layout: schema
name: UpdateTLSInspectionConfigurationRequest
properties_list:
- description: ''
  name: TLSInspectionConfigurationArn
  type: object
- description: ''
  name: TLSInspectionConfigurationName
  type: object
- description: ''
  name: TLSInspectionConfiguration
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: EncryptionConfiguration
  type: object
- description: ''
  name: UpdateToken
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-update-tls-inspection-configuration-request-schema.json
slug: openapi-update-tls-inspection-configuration-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-update-tls-inspection-configuration-request-schema.json\",\n  \"title\": \"UpdateTLSInspectionConfigurationRequest\",\n  \"description\": \"UpdateTLSInspectionConfigurationRequest schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TLSInspectionConfigurationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the TLS inspection configuration.\"\n        }\n      ]\n    },\n    \"TLSInspectionConfigurationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The descriptive name of the TLS inspection configuration. You can't\
  \ change the name of a TLS inspection configuration after you create it.\"\n        }\n      ]\n    },\n    \"TLSInspectionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TLSInspectionConfiguration\"\n        },\n        {\n          \"description\": \"<p>The object that defines a TLS inspection configuration. This, along with <a>TLSInspectionConfigurationResponse</a>, define the TLS inspection configuration. You can retrieve all objects for a TLS inspection configuration by calling <a>DescribeTLSInspectionConfiguration</a>. </p> <p>Network Firewall uses a TLS inspection configuration to decrypt traffic. Network Firewall re-encrypts the traffic before sending it to its destination.</p> <p>To use a TLS inspection configuration, you add it to a Network Firewall firewall policy, then you apply the firewall policy to a firewall. Network Firewall acts as a proxy service to decrypt and inspect inbound traffic. You can reference a TLS inspection configuration\
  \ from more than one firewall policy, and you can use a firewall policy in more than one firewall. For more information about using TLS inspection configurations, see <a href=\\\"https://docs.aws.amazon.com/network-firewall/latest/developerguide/tls-inspection.html\\\">Decrypting SSL/TLS traffic with TLS inspection configurations</a> in the <i>Network Firewall Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the TLS inspection configuration. \"\n        }\n      ]\n    },\n    \"EncryptionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionConfiguration\"\n        },\n        {\n          \"description\": \"A complex type that contains the Amazon Web Services KMS encryption configuration settings for your TLS inspection configuration.\"\n        }\n\
  \      ]\n    },\n    \"UpdateToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateToken\"\n        },\n        {\n          \"description\": \"<p>A token used for optimistic locking. Network Firewall returns a token to your requests that access the TLS inspection configuration. The token marks the state of the TLS inspection configuration resource at the time of the request. </p> <p>To make changes to the TLS inspection configuration, you provide the token in your request. Network Firewall uses the token to ensure that the TLS inspection configuration hasn't changed since you last retrieved it. If it has changed, the operation fails with an <code>InvalidTokenException</code>. If this happens, retrieve the TLS inspection configuration again to get a current copy of it with a current token. Reapply your changes as needed, then try the operation again using the new token. </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TLSInspectionConfiguration\"\
  ,\n    \"UpdateToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-update-tls-inspection-configuration-request-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: UpdateTLSInspectionConfigurationRequest
---
