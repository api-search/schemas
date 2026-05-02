---
description: Schema for Windows ML machine learning models and evaluation results as defined by the Windows.AI.MachineLearning namespace. Covers LearningModel, LearningModelSession, LearningModelBinding, feature descriptors, and evaluation results.
layout: schema
name: Windows 10 Machine Learning Model
properties_list:
- description: Model name from ONNX metadata
  name: name
  type: string
- description: Model author
  name: author
  type: string
- description: Model domain (e.g., image classification, NLP)
  name: domain
  type: string
- description: Model description
  name: description
  type: string
- description: Model version number
  name: version
  type: integer
- description: Input feature descriptors
  name: inputFeatures
  type: array
- description: Output feature descriptors
  name: outputFeatures
  type: array
- description: Custom metadata key-value pairs from the ONNX model
  name: metadata
  type: object
provider_name: Microsoft Windows 10
provider_slug: microsoft-windows-10
schema_file: json-schema/microsoft-windows-10-ml-model-schema.json
slug: microsoft-windows-10-ml-model
source_filename: microsoft-windows-10-ml-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.microsoft.com/schemas/windows-10/ml-model.json\",\n  \"title\": \"Windows 10 Machine Learning Model\",\n  \"description\": \"Schema for Windows ML machine learning models and evaluation results as defined by the Windows.AI.MachineLearning namespace. Covers LearningModel, LearningModelSession, LearningModelBinding, feature descriptors, and evaluation results.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Model name from ONNX metadata\"\n    },\n    \"author\": {\n      \"type\": \"string\",\n      \"description\": \"Model author\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Model domain (e.g., image classification, NLP)\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Model description\"\n    },\n    \"version\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"Model version number\"\n    },\n    \"inputFeatures\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/FeatureDescriptor\"\n      },\n      \"description\": \"Input feature descriptors\"\n    },\n    \"outputFeatures\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/FeatureDescriptor\"\n      },\n      \"description\": \"Output feature descriptors\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Custom metadata key-value pairs from the ONNX model\"\n    }\n  },\n  \"required\": [\"name\", \"inputFeatures\", \"outputFeatures\"],\n  \"$defs\": {\n    \"FeatureDescriptor\": {\n      \"type\": \"object\",\n      \"description\": \"Describes an input or output feature of a model (ILearningModelFeatureDescriptor)\",\n      \"properties\": {\n        \"name\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"Feature name\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Feature description\"\n        },\n        \"kind\": {\n          \"type\": \"string\",\n          \"enum\": [\"Tensor\", \"Sequence\", \"Map\", \"Image\"],\n          \"description\": \"Feature kind (LearningModelFeatureKind)\"\n        },\n        \"isRequired\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the feature is required for evaluation\"\n        },\n        \"tensorDescriptor\": {\n          \"$ref\": \"#/$defs/TensorFeatureDescriptor\"\n        },\n        \"imageDescriptor\": {\n          \"$ref\": \"#/$defs/ImageFeatureDescriptor\"\n        },\n        \"mapDescriptor\": {\n          \"$ref\": \"#/$defs/MapFeatureDescriptor\"\n        },\n        \"sequenceDescriptor\": {\n          \"$ref\": \"#/$defs/SequenceFeatureDescriptor\"\n        }\n      },\n      \"required\": [\"name\",\
  \ \"kind\"]\n    },\n    \"TensorFeatureDescriptor\": {\n      \"type\": \"object\",\n      \"description\": \"Descriptor for tensor features (TensorFeatureDescriptor class)\",\n      \"properties\": {\n        \"tensorKind\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Undefined\", \"Float\", \"UInt8\", \"Int8\", \"UInt16\", \"Int16\",\n            \"Int32\", \"Int64\", \"String\", \"Boolean\", \"Float16\", \"Double\",\n            \"UInt32\", \"UInt64\", \"Complex64\", \"Complex128\"\n          ],\n          \"description\": \"Tensor element data type (TensorKind)\"\n        },\n        \"shape\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"integer\"\n          },\n          \"description\": \"Tensor dimensions (-1 for variable dimensions)\"\n        }\n      },\n      \"required\": [\"tensorKind\", \"shape\"]\n    },\n    \"ImageFeatureDescriptor\": {\n      \"type\": \"object\",\n      \"description\": \"Descriptor\
  \ for image features (ImageFeatureDescriptor class)\",\n      \"properties\": {\n        \"bitmapAlphaMode\": {\n          \"type\": \"string\",\n          \"enum\": [\"Premultiplied\", \"Straight\", \"Ignore\"],\n          \"description\": \"Alpha channel mode\"\n        },\n        \"bitmapPixelFormat\": {\n          \"type\": \"string\",\n          \"enum\": [\"Unknown\", \"Rgba16\", \"Rgba8\", \"Gray16\", \"Gray8\", \"Bgra8\", \"Nv12\", \"P010\", \"Yuy2\"],\n          \"description\": \"Pixel format\"\n        },\n        \"height\": {\n          \"type\": \"integer\",\n          \"description\": \"Image height in pixels\"\n        },\n        \"width\": {\n          \"type\": \"integer\",\n          \"description\": \"Image width in pixels\"\n        }\n      },\n      \"required\": [\"bitmapPixelFormat\", \"height\", \"width\"]\n    },\n    \"MapFeatureDescriptor\": {\n      \"type\": \"object\",\n      \"description\": \"Descriptor for map features (MapFeatureDescriptor class)\"\
  ,\n      \"properties\": {\n        \"keyKind\": {\n          \"type\": \"string\",\n          \"enum\": [\"Float\", \"Int64\", \"String\", \"Double\"],\n          \"description\": \"Map key data type\"\n        },\n        \"valueDescriptor\": {\n          \"$ref\": \"#/$defs/FeatureDescriptor\"\n        }\n      },\n      \"required\": [\"keyKind\"]\n    },\n    \"SequenceFeatureDescriptor\": {\n      \"type\": \"object\",\n      \"description\": \"Descriptor for sequence features (SequenceFeatureDescriptor class)\",\n      \"properties\": {\n        \"elementDescriptor\": {\n          \"$ref\": \"#/$defs/FeatureDescriptor\"\n        }\n      }\n    },\n    \"EvaluationResult\": {\n      \"type\": \"object\",\n      \"description\": \"Result of a model evaluation (LearningModelEvaluationResult class)\",\n      \"properties\": {\n        \"correlationId\": {\n          \"type\": \"string\",\n          \"description\": \"Correlation identifier for tracking\"\n        },\n        \"errorStatus\"\
  : {\n          \"type\": \"integer\",\n          \"description\": \"Error status code (0 for success)\"\n        },\n        \"succeeded\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether evaluation succeeded\"\n        },\n        \"outputs\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true,\n          \"description\": \"Map of output feature names to their values\"\n        }\n      },\n      \"required\": [\"succeeded\"]\n    },\n    \"LearningModelDevice\": {\n      \"type\": \"object\",\n      \"description\": \"Device used for model evaluation (LearningModelDevice class)\",\n      \"properties\": {\n        \"deviceKind\": {\n          \"type\": \"string\",\n          \"enum\": [\"Default\", \"Cpu\", \"DirectX\", \"DirectXHighPerformance\", \"DirectXMinPower\"],\n          \"description\": \"Device type (LearningModelDeviceKind)\"\n        },\n        \"adapterId\": {\n          \"type\": \"object\",\n          \"properties\"\
  : {\n            \"highPart\": { \"type\": \"integer\" },\n            \"lowPart\": { \"type\": \"integer\" }\n          },\n          \"description\": \"GPU adapter identifier (for DirectX devices)\"\n        }\n      },\n      \"required\": [\"deviceKind\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/json-schema/microsoft-windows-10-ml-model-schema.json
tags:
- Desktop
- Operating System
- UWP
- Win32
- Windows
title: Windows 10 Machine Learning Model
---
