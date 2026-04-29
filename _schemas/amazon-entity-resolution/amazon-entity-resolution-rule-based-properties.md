---
description: An object which defines the list of matching rules to run and has a field <code>Rules</code>, which is a list of rule objects.
layout: schema
name: RuleBasedProperties
properties_list:
- description: ''
  name: attributeMatchingModel
  type: object
- description: ''
  name: rules
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-rule-based-properties-schema.json
slug: amazon-entity-resolution-rule-based-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-rule-based-properties-schema.json\",\n  \"title\": \"RuleBasedProperties\",\n  \"description\": \"An object which defines the list of matching rules to run and has a field <code>Rules</code>, which is a list of rule objects.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributeMatchingModel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeMatchingModel\"\n        },\n        {\n          \"description\": \"You can either choose <code>ONE_TO_ONE</code> or <code>MANY_TO_MANY</code> as the AttributeMatchingModel. When choosing <code>MANY_TO_MANY</code>, the system can match attribute across the sub-types of an attribute type. For example, if the value of the Email field of Profile A and the value of BusinessEmail field of\
  \ Profile B matches, the two profiles are matched on the Email type. When choosing <code>ONE_TO_ONE</code> the system can only match if the sub-types are exact matches. For example, only when the value of the Email field of Profile A and the value of the Email field of Profile B matches, the two profiles are matched on the Email type.\"\n        }\n      ]\n    },\n    \"rules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleBasedPropertiesRulesList\"\n        },\n        {\n          \"description\": \"A list of Rule objects, each of which have fields <code>RuleName</code> and <code>MatchingKeys</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"attributeMatchingModel\",\n    \"rules\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-rule-based-properties-schema.json
tags:
- Amazon Web Services
- AWS
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: RuleBasedProperties
---
