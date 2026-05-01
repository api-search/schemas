---
description: Configuration settings for the handling of the stateful rule groups in a firewall policy.
layout: schema
name: StatefulEngineOptions
properties_list:
- description: ''
  name: RuleOrder
  type: object
- description: ''
  name: StreamExceptionPolicy
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-stateful-engine-options-schema.json
slug: openapi-stateful-engine-options
source_filename: openapi-stateful-engine-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-stateful-engine-options-schema.json\",\n  \"title\": \"StatefulEngineOptions\",\n  \"description\": \"Configuration settings for the handling of the stateful rule groups in a firewall policy. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuleOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleOrder\"\n        },\n        {\n          \"description\": \"Indicates how to manage the order of stateful rule evaluation for the policy. <code>DEFAULT_ACTION_ORDER</code> is the default behavior. Stateful rules are provided to the rule engine as Suricata compatible strings, and Suricata evaluates them based on certain settings. For more information, see <a href=\\\"https://docs.aws.amazon.com/network-firewall/latest/developerguide/suricata-rule-evaluation-order.html\\\
  \">Evaluation order for stateful rules</a> in the <i>Network Firewall Developer Guide</i>. \"\n        }\n      ]\n    },\n    \"StreamExceptionPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamExceptionPolicy\"\n        },\n        {\n          \"description\": \"<p>Configures how Network Firewall processes traffic when a network connection breaks midstream. Network connections can break due to disruptions in external networks or within the firewall itself.</p> <ul> <li> <p> <code>DROP</code> - Network Firewall fails closed and drops all subsequent traffic going to the firewall. This is the default behavior.</p> </li> <li> <p> <code>CONTINUE</code> - Network Firewall continues to apply rules to the subsequent traffic without context from traffic before the break. This impacts the behavior of rules that depend on this context. For example, if you have a stateful rule to <code>drop http</code> traffic, Network Firewall won't match the traffic for\
  \ this rule because the service won't have the context from session initialization defining the application layer protocol as HTTP. However, this behavior is rule dependent\\u2014a TCP-layer rule using a <code>flow:stateless</code> rule would still match, as would the <code>aws:drop_strict</code> default action.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-stateful-engine-options-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: StatefulEngineOptions
---
