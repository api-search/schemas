---
description: A single Suricata rules specification, for use in a stateful rule group. Use this option to specify a simple Suricata rule with protocol, source and destination, ports, direction, and rule options. For information about the Suricata <code>Rules</code> format, see <a href="https://suricata.readthedocs.iorules/intro.html#">Rules Format</a>.
layout: schema
name: StatefulRule
properties_list:
- description: ''
  name: Action
  type: object
- description: ''
  name: Header
  type: object
- description: ''
  name: RuleOptions
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-stateful-rule-schema.json
slug: openapi-stateful-rule
source_filename: openapi-stateful-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-stateful-rule-schema.json\",\n  \"title\": \"StatefulRule\",\n  \"description\": \"A single Suricata rules specification, for use in a stateful rule group. Use this option to specify a simple Suricata rule with protocol, source and destination, ports, direction, and rule options. For information about the Suricata <code>Rules</code> format, see <a href=\\\"https://suricata.readthedocs.iorules/intro.html#\\\">Rules Format</a>. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatefulAction\"\n        },\n        {\n          \"description\": \"<p>Defines what Network Firewall should do with the packets in a traffic flow when the flow matches the stateful rule criteria. For all actions, Network\
  \ Firewall performs the specified action and discontinues stateful inspection of the traffic flow. </p> <p>The actions for a stateful rule are defined as follows: </p> <ul> <li> <p> <b>PASS</b> - Permits the packets to go to the intended destination.</p> </li> <li> <p> <b>DROP</b> - Blocks the packets from going to the intended destination and sends an alert log message, if alert logging is configured in the <a>Firewall</a> <a>LoggingConfiguration</a>. </p> </li> <li> <p> <b>ALERT</b> - Permits the packets to go to the intended destination and sends an alert log message, if alert logging is configured in the <a>Firewall</a> <a>LoggingConfiguration</a>. </p> <p>You can use this action to test a rule that you intend to use to drop traffic. You can enable the rule with <code>ALERT</code> action, verify in the logs that the rule is filtering as you want, then change the action to <code>DROP</code>.</p> </li> <li> <p> <b>REJECT</b> - Drops TCP traffic that matches the conditions of the stateful\
  \ rule, and sends a TCP reset packet back to sender of the packet. A TCP reset packet is a packet with no payload and a <code>RST</code> bit contained in the TCP header flags. Also sends an alert log mesage if alert logging is configured in the <a>Firewall</a> <a>LoggingConfiguration</a>.</p> <p> <code>REJECT</code> isn't currently available for use with IMAP and FTP protocols.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Header\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Header\"\n        },\n        {\n          \"description\": \"The stateful inspection criteria for this rule, used to inspect traffic flows. \"\n        }\n      ]\n    },\n    \"RuleOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleOptions\"\n        },\n        {\n          \"description\": \"Additional options for the rule. These are the Suricata <code>RuleOptions</code> settings.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"Action\",\n    \"Header\",\n    \"RuleOptions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-stateful-rule-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: StatefulRule
---
