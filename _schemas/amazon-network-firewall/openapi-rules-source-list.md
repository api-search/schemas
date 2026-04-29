---
description: <p>Stateful inspection criteria for a domain list rule group. </p> <p>For HTTPS traffic, domain filtering is SNI-based. It uses the server name indicator extension of the TLS handshake.</p> <p>By default, Network Firewall domain list inspection only includes traffic coming from the VPC where you deploy the firewall. To inspect traffic from IP addresses outside of the deployment VPC, you set the <code>HOME_NET</code> rule variable to include the CIDR range of the deployment VPC plus the other CIDR ranges. For more information, see <a>RuleVariables</a> in this guide and <a href="https://docs.aws.amazon.com/network-firewall/latest/developerguide/stateful-rule-groups-domain-names.html">Stateful domain list rule groups in Network Firewall</a> in the <i>Network Firewall Developer Guide</i>.</p>
layout: schema
name: RulesSourceList
properties_list:
- description: ''
  name: Targets
  type: object
- description: ''
  name: TargetTypes
  type: object
- description: ''
  name: GeneratedRulesType
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-rules-source-list-schema.json
slug: openapi-rules-source-list
source_filename: openapi-rules-source-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-rules-source-list-schema.json\",\n  \"title\": \"RulesSourceList\",\n  \"description\": \"<p>Stateful inspection criteria for a domain list rule group. </p> <p>For HTTPS traffic, domain filtering is SNI-based. It uses the server name indicator extension of the TLS handshake.</p> <p>By default, Network Firewall domain list inspection only includes traffic coming from the VPC where you deploy the firewall. To inspect traffic from IP addresses outside of the deployment VPC, you set the <code>HOME_NET</code> rule variable to include the CIDR range of the deployment VPC plus the other CIDR ranges. For more information, see <a>RuleVariables</a> in this guide and <a href=\\\"https://docs.aws.amazon.com/network-firewall/latest/developerguide/stateful-rule-groups-domain-names.html\\\">Stateful domain\
  \ list rule groups in Network Firewall</a> in the <i>Network Firewall Developer Guide</i>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Targets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleTargets\"\n        },\n        {\n          \"description\": \"<p>The domains that you want to inspect for in your traffic flows. Valid domain specifications are the following:</p> <ul> <li> <p>Explicit names. For example, <code>abc.example.com</code> matches only the domain <code>abc.example.com</code>.</p> </li> <li> <p>Names that use a domain wildcard, which you indicate with an initial '<code>.</code>'. For example,<code>.example.com</code> matches <code>example.com</code> and matches all subdomains of <code>example.com</code>, such as <code>abc.example.com</code> and <code>www.example.com</code>. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"TargetTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetTypes\"\
  \n        },\n        {\n          \"description\": \"The protocols you want to inspect. Specify <code>TLS_SNI</code> for <code>HTTPS</code>. Specify <code>HTTP_HOST</code> for <code>HTTP</code>. You can specify either or both. \"\n        }\n      ]\n    },\n    \"GeneratedRulesType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GeneratedRulesType\"\n        },\n        {\n          \"description\": \"Whether you want to allow or deny access to the domains in your target list.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Targets\",\n    \"TargetTypes\",\n    \"GeneratedRulesType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-rules-source-list-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: RulesSourceList
---
