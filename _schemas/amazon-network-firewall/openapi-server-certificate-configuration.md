---
description: <p>Configures the associated Certificate Manager Secure Sockets Layer/Transport Layer Security (SSL/TLS) server certificates and scope settings Network Firewall uses to decrypt traffic in a <a>TLSInspectionConfiguration</a>. For information about working with SSL/TLS certificates for TLS inspection, see <a href="https://docs.aws.amazon.com/network-firewall/latest/developerguide/tls-inspection-certificate-requirements.html"> Requirements for using SSL/TLS server certficiates with TLS inspection configurations</a> in the <i>Network Firewall Developer Guide</i>.</p> <note> <p>If a server certificate that's associated with your <a>TLSInspectionConfiguration</a> is revoked, deleted, or expired it can result in client-side TLS errors.</p> </note>
layout: schema
name: ServerCertificateConfiguration
properties_list:
- description: ''
  name: ServerCertificates
  type: object
- description: ''
  name: Scopes
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-server-certificate-configuration-schema.json
slug: openapi-server-certificate-configuration
source_filename: openapi-server-certificate-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-server-certificate-configuration-schema.json\",\n  \"title\": \"ServerCertificateConfiguration\",\n  \"description\": \"<p>Configures the associated Certificate Manager Secure Sockets Layer/Transport Layer Security (SSL/TLS) server certificates and scope settings Network Firewall uses to decrypt traffic in a <a>TLSInspectionConfiguration</a>. For information about working with SSL/TLS certificates for TLS inspection, see <a href=\\\"https://docs.aws.amazon.com/network-firewall/latest/developerguide/tls-inspection-certificate-requirements.html\\\"> Requirements for using SSL/TLS server certficiates with TLS inspection configurations</a> in the <i>Network Firewall Developer Guide</i>.</p> <note> <p>If a server certificate that's associated with your <a>TLSInspectionConfiguration</a> is revoked,\
  \ deleted, or expired it can result in client-side TLS errors.</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServerCertificates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServerCertificates\"\n        },\n        {\n          \"description\": \"The list of a server certificate configuration's Certificate Manager SSL/TLS certificates.\"\n        }\n      ]\n    },\n    \"Scopes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServerCertificateScopes\"\n        },\n        {\n          \"description\": \"A list of a server certificate configuration's scopes.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-server-certificate-configuration-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: ServerCertificateConfiguration
---
