---
description: Schema for a machine learning model hosted on the Hugging Face Hub, including metadata, configuration, and repository information.
layout: schema
name: Hugging Face Model
properties_list:
- description: Internal unique identifier for the model
  name: _id
  type: string
- description: Model repository ID in the format author/model-name or model-name
  name: id
  type: string
- description: Alias for the model repository ID
  name: modelId
  type: string
- description: Author or organization that owns the model
  name: author
  type: string
- description: Latest Git commit SHA of the model repository
  name: sha
  type: string
- description: Timestamp of the last modification to the repository
  name: lastModified
  type: string
- description: Timestamp when the model repository was created
  name: createdAt
  type: string
- description: Whether the model repository is private
  name: private
  type: boolean
- description: Whether the model has been disabled
  name: disabled
  type: boolean
- description: Access gating configuration. False means no gating, 'auto' or 'manual' indicates gated access.
  name: gated
  type: object
- description: The primary task/pipeline this model is designed for
  name: pipeline_tag
  type: string
- description: Tags associated with the model including library, language, license, and custom tags
  name: tags
  type: array
- description: Primary ML library used by the model
  name: library_name
  type: string
- description: Total number of downloads in the last 30 days
  name: downloads
  type: integer
- description: Total number of all-time downloads
  name: downloadsAllTime
  type: integer
- description: Total number of likes/favorites
  name: likes
  type: integer
- description: List of files in the model repository
  name: siblings
  type: array
- description: List of Space IDs that use this model
  name: spaces
  type: array
- description: Safetensors metadata including parameter counts
  name: safetensors
  type: object
- description: Model configuration from config.json
  name: config
  type: object
- description: Parsed metadata from the model card (README.md YAML front matter)
  name: cardData
  type: object
- description: Transformers library-specific information
  name: transformersInfo
  type: object
- description: Widget example data for the model card inference widget
  name: widgetData
  type: array
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-model-schema.json
slug: hugging-face-model
source_filename: hugging-face-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://huggingface.co/schemas/model.json\",\n  \"title\": \"Hugging Face Model\",\n  \"description\": \"Schema for a machine learning model hosted on the Hugging Face Hub, including metadata, configuration, and repository information.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\"\n  ],\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Internal unique identifier for the model\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Model repository ID in the format author/model-name or model-name\",\n      \"examples\": [\n        \"bert-base-uncased\",\n        \"meta-llama/Llama-3-70b-chat-hf\",\n        \"openai/whisper-large-v3\"\n      ]\n    },\n    \"modelId\": {\n      \"type\": \"string\",\n      \"description\": \"Alias for the model repository ID\"\n    },\n    \"author\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"Author or organization that owns the model\",\n      \"examples\": [\n        \"meta-llama\",\n        \"google\",\n        \"microsoft\"\n      ]\n    },\n    \"sha\": {\n      \"type\": \"string\",\n      \"description\": \"Latest Git commit SHA of the model repository\",\n      \"pattern\": \"^[0-9a-f]{40}$\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last modification to the repository\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the model repository was created\"\n    },\n    \"private\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the model repository is private\",\n      \"default\": false\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the model has been disabled\",\n      \"default\": false\n    },\n \
  \   \"gated\": {\n      \"oneOf\": [\n        {\n          \"type\": \"boolean\"\n        },\n        {\n          \"type\": \"string\",\n          \"enum\": [\n            \"auto\",\n            \"manual\"\n          ]\n        }\n      ],\n      \"description\": \"Access gating configuration. False means no gating, 'auto' or 'manual' indicates gated access.\"\n    },\n    \"pipeline_tag\": {\n      \"type\": \"string\",\n      \"description\": \"The primary task/pipeline this model is designed for\",\n      \"enum\": [\n        \"text-generation\",\n        \"text-classification\",\n        \"token-classification\",\n        \"question-answering\",\n        \"summarization\",\n        \"translation\",\n        \"fill-mask\",\n        \"text2text-generation\",\n        \"feature-extraction\",\n        \"sentence-similarity\",\n        \"zero-shot-classification\",\n        \"table-question-answering\",\n        \"conversational\",\n        \"image-classification\",\n        \"object-detection\"\
  ,\n        \"image-segmentation\",\n        \"image-to-text\",\n        \"text-to-image\",\n        \"text-to-video\",\n        \"text-to-speech\",\n        \"text-to-audio\",\n        \"automatic-speech-recognition\",\n        \"audio-classification\",\n        \"image-text-to-text\",\n        \"visual-question-answering\",\n        \"document-question-answering\",\n        \"depth-estimation\",\n        \"image-to-image\",\n        \"reinforcement-learning\",\n        \"robotics\",\n        \"video-classification\"\n      ]\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags associated with the model including library, language, license, and custom tags\",\n      \"examples\": [\n        [\n          \"transformers\",\n          \"pytorch\",\n          \"en\",\n          \"text-generation\",\n          \"license:apache-2.0\"\n        ]\n      ]\n    },\n    \"library_name\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Primary ML library used by the model\",\n      \"enum\": [\n        \"transformers\",\n        \"diffusers\",\n        \"timm\",\n        \"sentence-transformers\",\n        \"spacy\",\n        \"allennlp\",\n        \"flair\",\n        \"asteroid\",\n        \"espnet\",\n        \"speechbrain\",\n        \"adapter-transformers\",\n        \"fastai\",\n        \"stable-baselines3\",\n        \"ml-agents\",\n        \"open_clip\",\n        \"peft\",\n        \"setfit\",\n        \"span-marker\",\n        \"keras\",\n        \"sklearn\",\n        \"onnx\",\n        \"safetensors\",\n        \"tensorboard\"\n      ]\n    },\n    \"downloads\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of downloads in the last 30 days\",\n      \"minimum\": 0\n    },\n    \"downloadsAllTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of all-time downloads\",\n      \"minimum\": 0\n    },\n    \"likes\": {\n \
  \     \"type\": \"integer\",\n      \"description\": \"Total number of likes/favorites\",\n      \"minimum\": 0\n    },\n    \"siblings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"rfilename\": {\n            \"type\": \"string\",\n            \"description\": \"Relative file path within the repository\"\n          },\n          \"size\": {\n            \"type\": \"integer\",\n            \"description\": \"File size in bytes\"\n          },\n          \"blobId\": {\n            \"type\": \"string\",\n            \"description\": \"Git blob ID\"\n          },\n          \"lfs\": {\n            \"type\": \"object\",\n            \"description\": \"Git LFS metadata\",\n            \"properties\": {\n              \"sha256\": {\n                \"type\": \"string\",\n                \"description\": \"SHA-256 hash of the LFS file\"\n              },\n              \"size\": {\n                \"type\": \"integer\"\
  ,\n                \"description\": \"Actual file size in bytes\"\n              },\n              \"pointerSize\": {\n                \"type\": \"integer\",\n                \"description\": \"Size of the LFS pointer file\"\n              }\n            }\n          }\n        }\n      },\n      \"description\": \"List of files in the model repository\"\n    },\n    \"spaces\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of Space IDs that use this model\"\n    },\n    \"safetensors\": {\n      \"type\": \"object\",\n      \"description\": \"Safetensors metadata including parameter counts\",\n      \"properties\": {\n        \"parameters\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"integer\"\n          },\n          \"description\": \"Parameter counts by dtype (e.g., F16, BF16, F32)\"\n        },\n        \"total\": {\n          \"type\": \"integer\",\n\
  \          \"description\": \"Total parameter count\"\n        }\n      }\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"description\": \"Model configuration from config.json\",\n      \"properties\": {\n        \"architectures\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Model architecture classes\"\n        },\n        \"model_type\": {\n          \"type\": \"string\",\n          \"description\": \"Model type identifier (e.g., bert, gpt2, llama)\"\n        },\n        \"tokenizer_config\": {\n          \"type\": \"object\",\n          \"description\": \"Tokenizer configuration\"\n        }\n      }\n    },\n    \"cardData\": {\n      \"type\": \"object\",\n      \"description\": \"Parsed metadata from the model card (README.md YAML front matter)\",\n      \"properties\": {\n        \"language\": {\n          \"oneOf\": [\n            {\n              \"type\": \"string\"\n\
  \            },\n            {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            }\n          ],\n          \"description\": \"Language(s) supported by the model\"\n        },\n        \"license\": {\n          \"type\": \"string\",\n          \"description\": \"License identifier\",\n          \"examples\": [\n            \"apache-2.0\",\n            \"mit\",\n            \"cc-by-4.0\",\n            \"llama3\"\n          ]\n        },\n        \"library_name\": {\n          \"type\": \"string\"\n        },\n        \"tags\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"datasets\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Datasets used for training\"\n        },\n        \"metrics\": {\n          \"type\": \"array\",\n          \"\
  items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Evaluation metrics reported\"\n        },\n        \"base_model\": {\n          \"oneOf\": [\n            {\n              \"type\": \"string\"\n            },\n            {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            }\n          ],\n          \"description\": \"Base model(s) this model is derived from\"\n        },\n        \"pipeline_tag\": {\n          \"type\": \"string\"\n        },\n        \"model-index\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\"\n          },\n          \"description\": \"Evaluation results in model index format\"\n        }\n      }\n    },\n    \"transformersInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Transformers library-specific information\",\n      \"properties\": {\n        \"auto_model\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"AutoModel class to use (e.g., AutoModelForCausalLM)\"\n        },\n        \"pipeline_tag\": {\n          \"type\": \"string\",\n          \"description\": \"Pipeline tag inferred by transformers\"\n        },\n        \"processor\": {\n          \"type\": \"string\",\n          \"description\": \"Processor class to use\"\n        }\n      }\n    },\n    \"widgetData\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"Widget example data for the model card inference widget\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-model-schema.json
tags: []
title: Hugging Face Model
---
