---
description: The stateless or stateful rules definitions for use in a single rule group. Each rule group requires a single <code>RulesSource</code>. You can use an instance of this for either stateless rules or stateful rules.
layout: schema
name: RulesSource
properties_list:
- description: ''
  name: RulesString
  type: object
- description: ''
  name: RulesSourceList
  type: object
- description: ''
  name: StatefulRules
  type: object
- description: ''
  name: StatelessRulesAndCustomActions
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-rules-source-schema.json
slug: openapi-rules-source
source_filename: openapi-rules-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-rules-source-schema.json\",\n  \"title\": \"RulesSource\",\n  \"description\": \"The stateless or stateful rules definitions for use in a single rule group. Each rule group requires a single <code>RulesSource</code>. You can use an instance of this for either stateless rules or stateful rules. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RulesString\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RulesString\"\n        },\n        {\n          \"description\": \"<p>Stateful inspection criteria, provided in Suricata compatible intrusion prevention system (IPS) rules. Suricata is an open-source network IPS that includes a standard rule-based language for network traffic inspection.</p> <p>These rules contain the inspection criteria and the action\
  \ to take for traffic that matches the criteria, so this type of rule group doesn't have a separate action setting.</p>\"\n        }\n      ]\n    },\n    \"RulesSourceList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RulesSourceList\"\n        },\n        {\n          \"description\": \"Stateful inspection criteria for a domain list rule group. \"\n        }\n      ]\n    },\n    \"StatefulRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatefulRules\"\n        },\n        {\n          \"description\": \"An array of individual stateful rules inspection criteria to be used together in a stateful rule group. Use this option to specify simple Suricata rules with protocol, source and destination, ports, direction, and rule options. For information about the Suricata <code>Rules</code> format, see <a href=\\\"https://suricata.readthedocs.iorules/intro.html#\\\">Rules Format</a>. \"\n        }\n      ]\n    },\n    \"\
  StatelessRulesAndCustomActions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatelessRulesAndCustomActions\"\n        },\n        {\n          \"description\": \"Stateless inspection criteria to be used in a stateless rule group. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-rules-source-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: RulesSource
---
