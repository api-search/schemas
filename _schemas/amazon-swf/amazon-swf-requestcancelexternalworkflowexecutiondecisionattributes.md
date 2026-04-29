---
description: <p>Provides the details of the <code>RequestCancelExternalWorkflowExecution</code> decision.</p> <p> <b>Access Control</b> </p> <p>You can use IAM policies to control this decision's access to Amazon SWF resources as follows:</p> <ul> <li> <p>Use a <code>Resource</code> element with the domain name to limit the action to only specified domains.</p> </li> <li> <p>Use an <code>Action</code> element to allow or deny permission to call this action.</p> </li> <li> <p>You cannot use an IAM policy to constrain this action's parameters.</p> </li> </ul> <p>If the caller doesn't have sufficient permissions to invoke the action, or the parameter values fall outside the specified constraints, the action fails. The associated event attribute's <code>cause</code> parameter is set to <code>OPERATION_NOT_PERMITTED</code>. For details and example IAM policies, see <a href="https://docs.aws.amazon.com/amazonswf/latest/developerguide/swf-dev-iam.html">Using IAM to Manage Access to Amazon SWF Workflows</a>
  in the <i>Amazon SWF Developer Guide</i>.</p>
layout: schema
name: RequestCancelExternalWorkflowExecutionDecisionAttributes
properties_list:
- description: ''
  name: workflowId
  type: object
- description: ''
  name: runId
  type: object
- description: ''
  name: control
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-requestcancelexternalworkflowexecutiondecisionattributes-schema.json
slug: amazon-swf-requestcancelexternalworkflowexecutiondecisionattributes
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"workflowId\"\n  ],\n  \"properties\": {\n    \"workflowId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowId\"\n        },\n        {\n          \"description\": \" The <code>workflowId</code> of the external workflow execution to cancel.\"\n        }\n      ]\n    },\n    \"runId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowRunIdOptional\"\n        },\n        {\n          \"description\": \"The <code>runId</code> of the external workflow execution to cancel.\"\n        }\n      ]\n    },\n    \"control\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"The data attached to the event that can be used by the decider in subsequent workflow tasks.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"<p>Provides the details of the <code>RequestCancelExternalWorkflowExecution</code>\
  \ decision.</p> <p> <b>Access Control</b> </p> <p>You can use IAM policies to control this decision's access to Amazon SWF resources as follows:</p> <ul> <li> <p>Use a <code>Resource</code> element with the domain name to limit the action to only specified domains.</p> </li> <li> <p>Use an <code>Action</code> element to allow or deny permission to call this action.</p> </li> <li> <p>You cannot use an IAM policy to constrain this action's parameters.</p> </li> </ul> <p>If the caller doesn't have sufficient permissions to invoke the action, or the parameter values fall outside the specified constraints, the action fails. The associated event attribute's <code>cause</code> parameter is set to <code>OPERATION_NOT_PERMITTED</code>. For details and example IAM policies, see <a href=\\\"https://docs.aws.amazon.com/amazonswf/latest/developerguide/swf-dev-iam.html\\\">Using IAM to Manage Access to Amazon SWF Workflows</a> in the <i>Amazon SWF Developer Guide</i>.</p>\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\
  ,\n  \"title\": \"RequestCancelExternalWorkflowExecutionDecisionAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-requestcancelexternalworkflowexecutiondecisionattributes-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: RequestCancelExternalWorkflowExecutionDecisionAttributes
---
