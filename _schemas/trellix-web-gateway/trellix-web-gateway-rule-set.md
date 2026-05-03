---
description: Represents a policy rule set configured on the Trellix Web Gateway, containing ordered rules with conditions and actions for web traffic processing.
layout: schema
name: Trellix Web Gateway Rule Set
properties_list:
- description: Unique identifier for the rule set
  name: id
  type: string
- description: Display name of the rule set
  name: name
  type: string
- description: Description of the rule set purpose
  name: description
  type: string
- description: Processing phase in which this rule set is evaluated
  name: type
  type: string
- description: Whether the rule set is currently active
  name: enabled
  type: boolean
- description: Processing order relative to other rule sets
  name: order
  type: integer
- description: Number of rules contained in this rule set
  name: ruleCount
  type: integer
- description: Ordered list of rules within this rule set
  name: rules
  type: array
provider_name: Trellix Web Gateway
provider_slug: trellix-web-gateway
schema_file: json-schema/trellix-web-gateway-rule-set-schema.json
slug: trellix-web-gateway-rule-set
source_filename: trellix-web-gateway-rule-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.trellix.com/schemas/web-gateway/rule-set.json\",\n  \"title\": \"Trellix Web Gateway Rule Set\",\n  \"description\": \"Represents a policy rule set configured on the Trellix Web Gateway, containing ordered rules with conditions and actions for web traffic processing.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the rule set\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the rule set\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the rule set purpose\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"request\", \"response\", \"error\"],\n      \"description\": \"Processing phase in which this rule set is evaluated\"\n    },\n    \"enabled\": {\n      \"type\"\
  : \"boolean\",\n      \"description\": \"Whether the rule set is currently active\"\n    },\n    \"order\": {\n      \"type\": \"integer\",\n      \"description\": \"Processing order relative to other rule sets\"\n    },\n    \"ruleCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of rules contained in this rule set\"\n    },\n    \"rules\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Rule\"\n      },\n      \"description\": \"Ordered list of rules within this rule set\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"type\", \"enabled\"],\n  \"$defs\": {\n    \"Rule\": {\n      \"type\": \"object\",\n      \"description\": \"An individual policy rule with a condition and action\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the rule\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Rule name\"\
  \n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Rule description\"\n        },\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the rule is active\"\n        },\n        \"order\": {\n          \"type\": \"integer\",\n          \"description\": \"Processing order within the rule set\"\n        },\n        \"condition\": {\n          \"$ref\": \"#/$defs/RuleCondition\"\n        },\n        \"action\": {\n          \"$ref\": \"#/$defs/RuleAction\"\n        }\n      },\n      \"required\": [\"id\", \"name\", \"enabled\", \"condition\", \"action\"]\n    },\n    \"RuleCondition\": {\n      \"type\": \"object\",\n      \"description\": \"Condition that determines when a rule matches\",\n      \"properties\": {\n        \"property\": {\n          \"type\": \"string\",\n          \"description\": \"Property to evaluate (e.g., URL.Host, URL.Categories, Antimalware.Infected, Client.IP)\"\n    \
  \    },\n        \"operator\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"equals\",\n            \"not_equals\",\n            \"contains\",\n            \"not_contains\",\n            \"matches\",\n            \"in_list\",\n            \"not_in_list\",\n            \"greater_than\",\n            \"less_than\"\n          ],\n          \"description\": \"Comparison operator\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"Value to compare against\"\n        },\n        \"listRef\": {\n          \"type\": \"string\",\n          \"description\": \"Reference to a custom list for list-based operations\"\n        }\n      },\n      \"required\": [\"property\", \"operator\"]\n    },\n    \"RuleAction\": {\n      \"type\": \"object\",\n      \"description\": \"Action to execute when a rule condition matches\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n   \
  \         \"allow\",\n            \"block\",\n            \"redirect\",\n            \"authenticate\",\n            \"log\",\n            \"continue\",\n            \"stop_rule_set\",\n            \"stop_cycle\"\n          ],\n          \"description\": \"Action type\"\n        },\n        \"blockTemplate\": {\n          \"type\": \"string\",\n          \"description\": \"Block page template to display when action is block\"\n        },\n        \"redirectUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to redirect to when action is redirect\"\n        }\n      },\n      \"required\": [\"type\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/trellix-web-gateway/refs/heads/main/json-schema/trellix-web-gateway-rule-set-schema.json
tags:
- Cybersecurity
- Data Loss Prevention
- Enterprise Security
- Malware Protection
- Network Security
- Threat Protection
- URL Filtering
- Web Gateway
title: Trellix Web Gateway Rule Set
---
