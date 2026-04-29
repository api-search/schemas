---
description: ''
layout: schema
name: CreateResponseRequest
properties_list:
- description: Model ID used to generate the response, like gpt-4o or o3. OpenAI offers a wide range of models with different capabilities, performance characteristics, and price points.
  name: model
  type: string
- description: Text, image, or file inputs to the model, used to generate a response. Can be a string for simple text input, or an array of input items for multi-turn and multimodal inputs.
  name: input
  type: string
- description: A system (or developer) message inserted at the beginning of the model's context. Use this for top-level guidance on the model's behavior, tone, or constraints.
  name: instructions
  type: string
- description: The unique ID of the previous response to the model. Use this to create multi-turn conversations. The model will use the previous response as context.
  name: previous_response_id
  type: string
- description: An upper bound for the number of tokens that can be generated for a response, including visible output tokens and reasoning tokens.
  name: max_output_tokens
  type: integer
- description: What sampling temperature to use, between 0 and 2. Higher values like 0.8 make the output more random, while lower values like 0.2 make it more focused and deterministic.
  name: temperature
  type: number
- description: An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass.
  name: top_p
  type: number
- description: An array of tools the model may use to generate a response. Supports built-in tools (web_search_preview, file_search, code_interpreter, computer_use_preview) and custom function tools.
  name: tools
  type: array
- description: How the model should select which tool to use. auto allows the model to decide, required forces the model to use a tool, none disables tool use.
  name: tool_choice
  type: string
- description: The truncation strategy to use for the model context. auto will use the model-defined default truncation strategy. disabled will error if the context exceeds the model's context window.
  name: truncation
  type: string
- description: Configuration for text response format.
  name: text
  type: object
- description: Configuration for reasoning models (o-series). Controls how much reasoning effort the model uses.
  name: reasoning
  type: object
- description: Whether to store the generated response for later retrieval via the GET /responses endpoint. Defaults to true.
  name: store
  type: boolean
- description: Set of 16 key-value pairs that can be attached to an object. Useful for storing additional information in a structured format.
  name: metadata
  type: object
- description: If set to true, the model response data will be streamed as server-sent events to the client.
  name: stream
  type: boolean
- description: Whether to allow the model to run tool calls in parallel.
  name: parallel_tool_calls
  type: boolean
- description: A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse.
  name: user
  type: string
provider_name: ChatGPT
provider_slug: chatgpt
schema_file: json-schema/chatgpt-responses-create-response-request-schema.json
slug: chatgpt-responses-create-response-request
source_filename: chatgpt-responses-create-response-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateResponseRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Model ID used to generate the response, like gpt-4o or o3.\\nOpenAI offers a wide range of models with different capabilities,\\nperformance characteristics, and price points.\\n\"\n    },\n    \"input\": {\n      \"type\": \"string\",\n      \"description\": \"Text, image, or file inputs to the model, used to generate\\na response. Can be a string for simple text input, or an\\narray of input items for multi-turn and multimodal inputs.\\n\"\n    },\n    \"instructions\": {\n      \"type\": \"string\",\n      \"description\": \"A system (or developer) message inserted at the beginning\\nof the model's context. Use this for top-level guidance\\non the model's behavior, tone, or constraints.\\n\"\n    },\n    \"previous_response_id\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The unique ID of the previous response to the model. Use\\nthis to create multi-turn conversations. The model will\\nuse the previous response as context.\\n\"\n    },\n    \"max_output_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"An upper bound for the number of tokens that can be generated\\nfor a response, including visible output tokens and reasoning\\ntokens.\\n\"\n    },\n    \"temperature\": {\n      \"type\": \"number\",\n      \"description\": \"What sampling temperature to use, between 0 and 2. Higher\\nvalues like 0.8 make the output more random, while lower\\nvalues like 0.2 make it more focused and deterministic.\\n\"\n    },\n    \"top_p\": {\n      \"type\": \"number\",\n      \"description\": \"An alternative to sampling with temperature, called nucleus\\nsampling, where the model considers the results of the\\ntokens with top_p probability mass.\\n\"\n    },\n    \"tools\": {\n      \"type\": \"array\",\n \
  \     \"description\": \"An array of tools the model may use to generate a response.\\nSupports built-in tools (web_search_preview, file_search,\\ncode_interpreter, computer_use_preview) and custom function\\ntools.\\n\"\n    },\n    \"tool_choice\": {\n      \"type\": \"string\",\n      \"description\": \"How the model should select which tool to use. auto allows\\nthe model to decide, required forces the model to use a\\ntool, none disables tool use.\\n\"\n    },\n    \"truncation\": {\n      \"type\": \"string\",\n      \"description\": \"The truncation strategy to use for the model context. auto\\nwill use the model-defined default truncation strategy.\\ndisabled will error if the context exceeds the model's\\ncontext window.\\n\"\n    },\n    \"text\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for text response format.\"\n    },\n    \"reasoning\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for reasoning models (o-series). Controls\\\
  nhow much reasoning effort the model uses.\\n\"\n    },\n    \"store\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to store the generated response for later retrieval\\nvia the GET /responses endpoint. Defaults to true.\\n\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Set of 16 key-value pairs that can be attached to an object.\\nUseful for storing additional information in a structured format.\\n\"\n    },\n    \"stream\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set to true, the model response data will be streamed\\nas server-sent events to the client.\\n\"\n    },\n    \"parallel_tool_calls\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to allow the model to run tool calls in parallel.\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier representing your end-user, which can\\nhelp OpenAI to monitor and detect abuse.\\n\"\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chatgpt/refs/heads/main/json-schema/chatgpt-responses-create-response-request-schema.json
tags:
- Agents
- AI
- ChatGPT
- Embeddings
- Fine-Tuning
- GPT-4
- GPT-5
- Language Model
- OpenAI
- Realtime
title: CreateResponseRequest
---
