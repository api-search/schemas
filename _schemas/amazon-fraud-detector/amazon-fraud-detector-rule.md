---
description: A Fraud Detector rule that maps model scores and event variables to outcomes.
layout: schema
name: Rule
properties_list:
- description: Unique rule identifier.
  name: ruleId
  type: string
- description: Detector this rule belongs to.
  name: detectorId
  type: string
- description: Version of the rule.
  name: ruleVersion
  type: string
- description: ''
  name: description
  type: string
- description: Rule expression language.
  name: language
  type: string
- description: Rule expression evaluated against event variables and model scores.
  name: expression
  type: string
- description: Outcomes triggered when the rule matches.
  name: outcomes
  type: array
- description: ''
  name: arn
  type: string
provider_name: Amazon Fraud Detector
provider_slug: amazon-fraud-detector
schema_file: json-schema/amazon-fraud-detector-rule-schema.json
slug: amazon-fraud-detector-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fraud-detector/refs/heads/main/json-schema/amazon-fraud-detector-rule-schema.json\",\n  \"title\": \"Rule\",\n  \"description\": \"A Fraud Detector rule that maps model scores and event variables to outcomes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ruleId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique rule identifier.\"\n    },\n    \"detectorId\": {\n      \"type\": \"string\",\n      \"description\": \"Detector this rule belongs to.\"\n    },\n    \"ruleVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Version of the rule.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"DETECTORPL\"\n      ],\n      \"description\": \"Rule expression language.\"\n    },\n    \"expression\": {\n     \
  \ \"type\": \"string\",\n      \"description\": \"Rule expression evaluated against event variables and model scores.\"\n    },\n    \"outcomes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Outcomes triggered when the rule matches.\"\n    },\n    \"arn\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"ruleId\",\n    \"detectorId\",\n    \"expression\",\n    \"language\",\n    \"outcomes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fraud-detector/refs/heads/main/json-schema/amazon-fraud-detector-rule-schema.json
tags:
- AWS
- Financial Services
- Fraud Detection
- Machine Learning
- Security
title: Rule
---
