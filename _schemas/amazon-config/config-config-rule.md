---
description: '<p>Config rules evaluate the configuration settings of your Amazon Web Services resources. A rule can run when Config detects a configuration change to an Amazon Web Services resource or at a periodic frequency that you choose (for example, every 24 hours). There are two types of rules: <i>Config Managed Rules</i> and <i>Config Custom Rules</i>.</p> <p>Config Managed Rules are predefined, customizable rules created by Config. For a list of managed rules, see <a href="https://docs.aws.amazon.com/config/latest/developerguide/managed-rules-by-aws-config.html">List of Config Managed Rules</a>.</p> <p>Config Custom Rules are rules that you create from scratch. There are two ways to create Config custom rules: with Lambda functions (<a href="https://docs.aws.amazon.com/config/latest/developerguide/gettingstarted-concepts.html#gettingstarted-concepts-function"> Lambda Developer Guide</a>) and with Guard (<a href="https://github.com/aws-cloudformation/cloudformation-guard">Guard GitHub
  Repository</a>), a policy-as-code language. Config custom rules created with Lambda are called <i>Config Custom Lambda Rules</i> and Config custom rules created with Guard are called <i>Config Custom Policy Rules</i>.</p> <p>For more information about developing and using Config rules, see <a href="https://docs.aws.amazon.com/config/latest/developerguide/evaluate-config.html">Evaluating Resource with Config Rules</a> in the <i>Config Developer Guide</i>.</p> <note> <p>You can use the Amazon Web Services CLI and Amazon Web Services SDKs if you want to create a rule that triggers evaluations for your resources when Config delivers the configuration snapshot. For more information, see <a>ConfigSnapshotDeliveryProperties</a>.</p> </note>'
layout: schema
name: ConfigRule
properties_list:
- description: ''
  name: ConfigRuleName
  type: object
- description: ''
  name: ConfigRuleArn
  type: object
- description: ''
  name: ConfigRuleId
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Scope
  type: object
- description: ''
  name: Source
  type: object
- description: ''
  name: InputParameters
  type: object
- description: ''
  name: MaximumExecutionFrequency
  type: object
- description: ''
  name: ConfigRuleState
  type: object
- description: ''
  name: CreatedBy
  type: object
- description: ''
  name: EvaluationModes
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-config-rule-schema.json
slug: config-config-rule
source_filename: config-config-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-config-rule-schema.json\",\n  \"title\": \"ConfigRule\",\n  \"description\": \"<p>Config rules evaluate the configuration settings of your Amazon Web Services resources. A rule can run when Config detects a configuration change to an Amazon Web Services resource or at a periodic frequency that you choose (for example, every 24 hours). There are two types of rules: <i>Config Managed Rules</i> and <i>Config Custom Rules</i>.</p> <p>Config Managed Rules are predefined, customizable rules created by Config. For a list of managed rules, see <a href=\\\"https://docs.aws.amazon.com/config/latest/developerguide/managed-rules-by-aws-config.html\\\">List of Config Managed Rules</a>.</p> <p>Config Custom Rules are rules that you create from scratch. There are two ways to create Config custom rules: with Lambda\
  \ functions (<a href=\\\"https://docs.aws.amazon.com/config/latest/developerguide/gettingstarted-concepts.html#gettingstarted-concepts-function\\\"> Lambda Developer Guide</a>) and with Guard (<a href=\\\"https://github.com/aws-cloudformation/cloudformation-guard\\\">Guard GitHub Repository</a>), a policy-as-code language. Config custom rules created with Lambda are called <i>Config Custom Lambda Rules</i> and Config custom rules created with Guard are called <i>Config Custom Policy Rules</i>.</p> <p>For more information about developing and using Config rules, see <a href=\\\"https://docs.aws.amazon.com/config/latest/developerguide/evaluate-config.html\\\">Evaluating Resource with Config Rules</a> in the <i>Config Developer Guide</i>.</p> <note> <p>You can use the Amazon Web Services CLI and Amazon Web Services SDKs if you want to create a rule that triggers evaluations for your resources when Config delivers the configuration snapshot. For more information, see <a>ConfigSnapshotDeliveryProperties</a>.</p>\
  \ </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRuleName\"\n        },\n        {\n          \"description\": \"The name that you assign to the Config rule. The name is required if you are adding a new rule.\"\n        }\n      ]\n    },\n    \"ConfigRuleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Config rule.\"\n        }\n      ]\n    },\n    \"ConfigRuleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit64\"\n        },\n        {\n          \"description\": \"The ID of the Config rule.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmptiableStringWithCharLimit256\"\n        },\n  \
  \      {\n          \"description\": \"The description that you provide for the Config rule.\"\n        }\n      ]\n    },\n    \"Scope\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scope\"\n        },\n        {\n          \"description\": \"<p>Defines which resources can trigger an evaluation for the rule. The scope can include one or more resource types, a combination of one resource type and one resource ID, or a combination of a tag key and value. Specify a scope to constrain the resources that can trigger an evaluation for the rule. If you do not specify a scope, evaluations are triggered when any resource in the recording group changes.</p> <note> <p>The scope can be empty. </p> </note>\"\n        }\n      ]\n    },\n    \"Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Source\"\n        },\n        {\n          \"description\": \"Provides the rule owner (<code>Amazon Web Services</code> for managed rules,\
  \ <code>CUSTOM_POLICY</code> for Custom Policy rules, and <code>CUSTOM_LAMBDA</code> for Custom Lambda rules), the rule identifier, and the notifications that cause the function to evaluate your Amazon Web Services resources.\"\n        }\n      ]\n    },\n    \"InputParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit1024\"\n        },\n        {\n          \"description\": \"A string, in JSON format, that is passed to the Config rule Lambda function.\"\n        }\n      ]\n    },\n    \"MaximumExecutionFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaximumExecutionFrequency\"\n        },\n        {\n          \"description\": \"<p>The maximum frequency with which Config runs evaluations for a rule. You can specify a value for <code>MaximumExecutionFrequency</code> when:</p> <ul> <li> <p>This is for an Config managed rule that is triggered at a periodic frequency.</p> </li> <li> <p>Your\
  \ custom rule is triggered when Config delivers the configuration snapshot. For more information, see <a>ConfigSnapshotDeliveryProperties</a>.</p> </li> </ul> <note> <p>By default, rules with a periodic trigger are evaluated every 24 hours. To change the frequency, specify a valid value for the <code>MaximumExecutionFrequency</code> parameter.</p> </note>\"\n        }\n      ]\n    },\n    \"ConfigRuleState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRuleState\"\n        },\n        {\n          \"description\": \"<p>Indicates whether the Config rule is active or is currently being deleted by Config. It can also indicate the evaluation status for the Config rule.</p> <p>Config sets the state of the rule to <code>EVALUATING</code> temporarily after you use the <code>StartConfigRulesEvaluation</code> request to evaluate your resources against the Config rule.</p> <p>Config sets the state of the rule to <code>DELETING_RESULTS</code> temporarily after\
  \ you use the <code>DeleteEvaluationResults</code> request to delete the current evaluation results for the Config rule.</p> <p>Config temporarily sets the state of a rule to <code>DELETING</code> after you use the <code>DeleteConfigRule</code> request to delete the rule. After Config deletes the rule, the rule and all of its evaluations are erased and are no longer available.</p>\"\n        }\n      ]\n    },\n    \"CreatedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"<p>Service principal name of the service that created the rule.</p> <note> <p>The field is populated only if the service-linked rule is created by a service. The field is empty if you create your own rule.</p> </note>\"\n        }\n      ]\n    },\n    \"EvaluationModes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EvaluationModes\"\n        },\n        {\n          \"description\"\
  : \"The modes the Config rule can be evaluated in. The valid values are distinct objects. By default, the value is Detective evaluation mode only.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Source\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-config-rule-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: ConfigRule
---
