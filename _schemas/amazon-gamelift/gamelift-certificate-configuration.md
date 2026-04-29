---
description: Determines whether a TLS/SSL certificate is generated for a fleet. This feature must be enabled when creating the fleet. All instances in a fleet share the same certificate. The certificate can be retrieved by calling the <a href="https://docs.aws.amazon.com/gamelift/latest/developerguide/reference-serversdk.html">Amazon GameLift Server SDK</a> operation <code>GetInstanceCertificate</code>.
layout: schema
name: CertificateConfiguration
properties_list:
- description: ''
  name: CertificateType
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-certificate-configuration-schema.json
slug: gamelift-certificate-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-certificate-configuration-schema.json\",\n  \"title\": \"CertificateConfiguration\",\n  \"description\": \"Determines whether a TLS/SSL certificate is generated for a fleet. This feature must be enabled when creating the fleet. All instances in a fleet share the same certificate. The certificate can be retrieved by calling the <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/reference-serversdk.html\\\">Amazon GameLift Server SDK</a> operation <code>GetInstanceCertificate</code>. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateType\"\n        },\n        {\n          \"description\": \"<p>Indicates whether a TLS/SSL certificate is generated for a fleet. </p>\
  \ <p>Valid values include: </p> <ul> <li> <p> <b>GENERATED</b> - Generate a TLS/SSL certificate for this fleet.</p> </li> <li> <p> <b>DISABLED</b> - (default) Do not generate a TLS/SSL certificate for this fleet. </p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CertificateType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-certificate-configuration-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: CertificateConfiguration
---
