---
description: Schema for a Junos OS security policy rule as configured on SRX Series firewalls and vSRX virtual firewalls. Security policies are the primary mechanism for controlling traffic flow between security zones on Juniper SRX platforms. Rules are organized in from-zone/to-zone pairs and evaluated in top-down order. Each rule matches traffic by source address, destination address, and application, then applies an action (permit, deny, reject) along with optional logging, counting, and UTM/IDP security profile enforcement. Policies are configured under the security policies hierarchy and can be managed via CLI, J-Web, Junos Space Security Director, or the REST/NETCONF API.
layout: schema
name: Junos Security Policy Rule
properties_list:
- description: Unique policy rule name within the from-zone/to-zone context. Maximum 63 characters.
  name: name
  type: string
- description: Policy rule description for documentation and audit purposes.
  name: description
  type: string
- description: Source security zone name. Traffic must originate from an interface bound to this zone.
  name: from_zone
  type: string
- description: Destination security zone name. Traffic must be destined for an interface bound to this zone.
  name: to_zone
  type: string
- description: Traffic match criteria. All criteria must match for the rule to apply.
  name: match
  type: object
- description: Action and service profile assignment when traffic matches the rule.
  name: then
  type: object
- description: Scheduler name for time-based policy activation. The rule is only active during the defined schedule windows.
  name: scheduler_name
  type: string
provider_name: Juniper Networks
provider_slug: juniper-networks
schema_file: json-schema/juniper-networks-junos-security-policy-schema.json
slug: juniper-networks-junos-security-policy
source_filename: juniper-networks-junos-security-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/json-schema/juniper-networks-junos-security-policy-schema.json\",\n  \"title\": \"Junos Security Policy Rule\",\n  \"description\": \"Schema for a Junos OS security policy rule as configured on SRX Series firewalls and vSRX virtual firewalls. Security policies are the primary mechanism for controlling traffic flow between security zones on Juniper SRX platforms. Rules are organized in from-zone/to-zone pairs and evaluated in top-down order. Each rule matches traffic by source address, destination address, and application, then applies an action (permit, deny, reject) along with optional logging, counting, and UTM/IDP security profile enforcement. Policies are configured under the security policies hierarchy and can be managed via CLI, J-Web, Junos Space Security Director, or the REST/NETCONF API.\",\n  \"type\":\
  \ \"object\",\n  \"required\": [\"name\", \"match\", \"then\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique policy rule name within the from-zone/to-zone context. Maximum 63 characters.\",\n      \"maxLength\": 63,\n      \"pattern\": \"^[a-zA-Z][a-zA-Z0-9._-]*$\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Policy rule description for documentation and audit purposes.\",\n      \"maxLength\": 900\n    },\n    \"from_zone\": {\n      \"type\": \"string\",\n      \"description\": \"Source security zone name. Traffic must originate from an interface bound to this zone.\"\n    },\n    \"to_zone\": {\n      \"type\": \"string\",\n      \"description\": \"Destination security zone name. Traffic must be destined for an interface bound to this zone.\"\n    },\n    \"match\": {\n      \"type\": \"object\",\n      \"description\": \"Traffic match criteria. All criteria must match for the rule to apply.\"\
  ,\n      \"properties\": {\n        \"source_address\": {\n          \"type\": \"array\",\n          \"description\": \"Source address match list. References address book entries defined in the from-zone. Use 'any' to match all source addresses.\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"default\": [\"any\"]\n        },\n        \"destination_address\": {\n          \"type\": \"array\",\n          \"description\": \"Destination address match list. References address book entries defined in the to-zone. Use 'any' to match all destination addresses.\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"default\": [\"any\"]\n        },\n        \"application\": {\n          \"type\": \"array\",\n          \"description\": \"Application match list. References predefined or custom application definitions that match traffic by protocol and port. Use 'any' to match all applications.\",\n          \"items\": {\n   \
  \         \"type\": \"string\"\n          },\n          \"default\": [\"any\"]\n        },\n        \"source_identity\": {\n          \"type\": \"array\",\n          \"description\": \"Source identity match list for user firewall (JIMS/Active Directory integrated) policies. References user, group, or role identities.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"dynamic_application\": {\n          \"type\": \"array\",\n          \"description\": \"Application identification match list for AppID-based policies on SRX4000+ platforms. References Juniper application signatures.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"required\": [\"source_address\", \"destination_address\", \"application\"]\n    },\n    \"then\": {\n      \"type\": \"object\",\n      \"description\": \"Action and service profile assignment when traffic matches the rule.\",\n      \"properties\": {\n        \"\
  action\": {\n          \"type\": \"string\",\n          \"enum\": [\"permit\", \"deny\", \"reject\"],\n          \"description\": \"Policy action. 'permit' allows traffic, 'deny' silently drops traffic, 'reject' drops traffic and sends an ICMP destination-unreachable or TCP RST.\"\n        },\n        \"log\": {\n          \"type\": \"object\",\n          \"description\": \"Logging configuration for matched traffic.\",\n          \"properties\": {\n            \"session_init\": {\n              \"type\": \"boolean\",\n              \"description\": \"Log at session initiation. Generates a log entry when the first packet of a new session matches this rule.\",\n              \"default\": false\n            },\n            \"session_close\": {\n              \"type\": \"boolean\",\n              \"description\": \"Log at session close. Generates a log entry with session summary when the session ends.\",\n              \"default\": false\n            }\n          }\n        },\n        \"\
  count\": {\n          \"type\": \"boolean\",\n          \"description\": \"Enable per-rule packet and byte counters.\",\n          \"default\": false\n        },\n        \"permit\": {\n          \"type\": \"object\",\n          \"description\": \"Additional options when action is permit.\",\n          \"properties\": {\n            \"application_services\": {\n              \"type\": \"object\",\n              \"description\": \"Security service profiles to apply to permitted traffic.\",\n              \"properties\": {\n                \"utm_policy\": {\n                  \"type\": \"string\",\n                  \"description\": \"Unified Threat Management policy name for content security (antivirus, web filtering, anti-spam, content filtering).\"\n                },\n                \"idp_policy\": {\n                  \"type\": \"string\",\n                  \"description\": \"Intrusion Detection and Prevention policy name.\"\n                },\n                \"ssl_proxy\": {\n\
  \                  \"type\": \"object\",\n                  \"description\": \"SSL forward proxy configuration for HTTPS inspection.\",\n                  \"properties\": {\n                    \"profile_name\": {\n                      \"type\": \"string\",\n                      \"description\": \"SSL proxy profile name.\"\n                    }\n                  }\n                },\n                \"application_firewall_rule_set\": {\n                  \"type\": \"string\",\n                  \"description\": \"Application firewall rule set name for Layer 7 application control.\"\n                }\n              }\n            },\n            \"tunnel\": {\n              \"type\": \"object\",\n              \"description\": \"IPsec tunnel encapsulation for VPN traffic.\",\n              \"properties\": {\n                \"ipsec_vpn\": {\n                  \"type\": \"string\",\n                  \"description\": \"IPsec VPN tunnel name.\"\n                },\n                \"\
  pair_policy\": {\n                  \"type\": \"string\",\n                  \"description\": \"Paired policy name for bidirectional VPN tunnels.\"\n                }\n              }\n            }\n          }\n        }\n      },\n      \"required\": [\"action\"]\n    },\n    \"scheduler_name\": {\n      \"type\": \"string\",\n      \"description\": \"Scheduler name for time-based policy activation. The rule is only active during the defined schedule windows.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/json-schema/juniper-networks-junos-security-policy-schema.json
tags:
- Automation
- Cloud
- Data Center
- Enterprise
- Networking
- SDN
- Security
title: Junos Security Policy Rule
---
