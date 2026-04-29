---
description: ''
layout: schema
name: CreateChatCompletionRequest
properties_list:
- description: ID of the model to use. See the model endpoint compatibility table for details on which models work with the Chat Completions API.
  name: model
  type: string
- description: A list of messages comprising the conversation so far. Depending on the model, different message types (modalities) are supported, like text, images, and audio.
  name: messages
  type: array
- description: Number between -2.0 and 2.0. Positive values penalize new tokens based on their existing frequency in the text so far, decreasing the model's likelihood to repeat the same line verbatim.
  name: frequency_penalty
  type: number
- description: Modify the likelihood of specified tokens appearing in the completion. Maps token IDs to bias values from -100 to 100.
  name: logit_bias
  type: object
- description: Whether to return log probabilities of the output tokens.
  name: logprobs
  type: boolean
- description: Number of most likely tokens to return at each position, each with an associated log probability. logprobs must be set to true if this parameter is used.
  name: top_logprobs
  type: integer
- description: An upper bound for the number of tokens that can be generated for a completion, including visible output tokens and reasoning tokens. Replaces the deprecated max_tokens parameter.
  name: max_completion_tokens
  type: integer
- description: How many chat completion choices to generate for each input message. Note that you will be charged based on the number of generated tokens across all choices.
  name: n
  type: integer
- description: Number between -2.0 and 2.0. Positive values penalize new tokens based on whether they appear in the text so far, increasing the model's likelihood to talk about new topics.
  name: presence_penalty
  type: number
- description: If specified, the system will make a best effort to sample deterministically, such that repeated requests with the same seed and parameters should return the same result.
  name: seed
  type: integer
- description: Up to 4 sequences where the API will stop generating further tokens.
  name: stop
  type: string
- description: 'If set, partial message deltas will be sent as server-sent events as they become available. The stream is terminated by a data: [DONE] message.'
  name: stream
  type: boolean
- description: Options for streaming responses.
  name: stream_options
  type: object
- description: What sampling temperature to use, between 0 and 2. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic.
  name: temperature
  type: number
- description: An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass.
  name: top_p
  type: number
- description: A list of tools the model may call. Currently, only functions are supported as a tool. Use this to provide a list of functions the model may generate JSON inputs for.
  name: tools
  type: array
- description: Controls which (if any) tool is called by the model. "none" means the model will not call any tool. "auto" means the model can pick between generating a message or calling one or more tools. "required
  name: tool_choice
  type: string
- description: Whether to enable parallel function calling during tool use.
  name: parallel_tool_calls
  type: boolean
- description: A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse.
  name: user
  type: string
- description: Whether or not to store the output of this chat completion request for use in the model distillation or evals products.
  name: store
  type: boolean
- description: Set of 16 key-value pairs that can be attached to an object. Useful for storing additional information in a structured format.
  name: metadata
  type: object
provider_name: ChatGPT
provider_slug: chatgpt
schema_file: json-schema/chatgpt-chat-completions-create-chat-completion-request-schema.json
slug: chatgpt-chat-completions-create-chat-completion-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateChatCompletionRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the model to use. See the model endpoint compatibility\\ntable for details on which models work with the Chat Completions API.\\n\"\n    },\n    \"messages\": {\n      \"type\": \"array\",\n      \"description\": \"A list of messages comprising the conversation so far.\\nDepending on the model, different message types (modalities)\\nare supported, like text, images, and audio.\\n\"\n    },\n    \"frequency_penalty\": {\n      \"type\": \"number\",\n      \"description\": \"Number between -2.0 and 2.0. Positive values penalize new tokens\\nbased on their existing frequency in the text so far, decreasing\\nthe model's likelihood to repeat the same line verbatim.\\n\"\n    },\n    \"logit_bias\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Modify the likelihood of specified tokens appearing in the\\ncompletion. Maps token IDs to bias values from -100 to 100.\\n\"\n    },\n    \"logprobs\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to return log probabilities of the output tokens.\\n\"\n    },\n    \"top_logprobs\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of most likely tokens to return at each position,\\neach with an associated log probability. logprobs must be\\nset to true if this parameter is used.\\n\"\n    },\n    \"max_completion_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"An upper bound for the number of tokens that can be generated\\nfor a completion, including visible output tokens and reasoning\\ntokens. Replaces the deprecated max_tokens parameter.\\n\"\n    },\n    \"n\": {\n      \"type\": \"integer\",\n      \"description\": \"How many chat completion choices to generate for each input\\nmessage. Note that you will be charged based\
  \ on the number\\nof generated tokens across all choices.\\n\"\n    },\n    \"presence_penalty\": {\n      \"type\": \"number\",\n      \"description\": \"Number between -2.0 and 2.0. Positive values penalize new tokens\\nbased on whether they appear in the text so far, increasing the\\nmodel's likelihood to talk about new topics.\\n\"\n    },\n    \"seed\": {\n      \"type\": \"integer\",\n      \"description\": \"If specified, the system will make a best effort to sample\\ndeterministically, such that repeated requests with the same\\nseed and parameters should return the same result.\\n\"\n    },\n    \"stop\": {\n      \"type\": \"string\",\n      \"description\": \"Up to 4 sequences where the API will stop generating further\\ntokens.\\n\"\n    },\n    \"stream\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set, partial message deltas will be sent as server-sent\\nevents as they become available. The stream is terminated by\\na data: [DONE] message.\\n\"\n    },\n\
  \    \"stream_options\": {\n      \"type\": \"object\",\n      \"description\": \"Options for streaming responses.\"\n    },\n    \"temperature\": {\n      \"type\": \"number\",\n      \"description\": \"What sampling temperature to use, between 0 and 2. Higher\\nvalues like 0.8 will make the output more random, while\\nlower values like 0.2 will make it more focused and deterministic.\\n\"\n    },\n    \"top_p\": {\n      \"type\": \"number\",\n      \"description\": \"An alternative to sampling with temperature, called nucleus\\nsampling, where the model considers the results of the tokens\\nwith top_p probability mass.\\n\"\n    },\n    \"tools\": {\n      \"type\": \"array\",\n      \"description\": \"A list of tools the model may call. Currently, only functions\\nare supported as a tool. Use this to provide a list of functions\\nthe model may generate JSON inputs for.\\n\"\n    },\n    \"tool_choice\": {\n      \"type\": \"string\",\n      \"description\": \"Controls which (if any)\
  \ tool is called by the model. \\\"none\\\"\\nmeans the model will not call any tool. \\\"auto\\\" means the\\nmodel can pick between generating a message or calling one\\nor more tools. \\\"required\\\" means the model must call one or\\nmore tools.\\n\"\n    },\n    \"parallel_tool_calls\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable parallel function calling during tool use.\\n\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier representing your end-user, which can\\nhelp OpenAI to monitor and detect abuse.\\n\"\n    },\n    \"store\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether or not to store the output of this chat completion\\nrequest for use in the model distillation or evals products.\\n\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Set of 16 key-value pairs that can be attached to an object.\\nUseful for storing additional information\
  \ in a structured format.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chatgpt/refs/heads/main/json-schema/chatgpt-chat-completions-create-chat-completion-request-schema.json
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
title: CreateChatCompletionRequest
---
