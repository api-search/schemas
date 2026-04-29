---
description: Provides information about a document classifier.
layout: schema
name: DocumentClassifierProperties
properties_list:
- description: ''
  name: DocumentClassifierArn
  type: object
- description: ''
  name: LanguageCode
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: Message
  type: object
- description: ''
  name: SubmitTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: TrainingStartTime
  type: object
- description: ''
  name: TrainingEndTime
  type: object
- description: ''
  name: InputDataConfig
  type: object
- description: ''
  name: OutputDataConfig
  type: object
- description: ''
  name: ClassifierMetadata
  type: object
- description: ''
  name: DataAccessRoleArn
  type: object
- description: ''
  name: VolumeKmsKeyId
  type: object
- description: ''
  name: VpcConfig
  type: object
- description: ''
  name: Mode
  type: object
- description: ''
  name: ModelKmsKeyId
  type: object
- description: ''
  name: VersionName
  type: object
- description: ''
  name: SourceModelArn
  type: object
- description: ''
  name: FlywheelArn
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-document-classifier-properties-schema.json
slug: openapi.yml-document-classifier-properties
source_filename: openapi.yml-document-classifier-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-classifier-properties-schema.json\",\n  \"title\": \"DocumentClassifierProperties\",\n  \"description\": \"Provides information about a document classifier.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DocumentClassifierArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentClassifierArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the document classifier.\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n          \"description\": \"The language code for the language of the documents that the classifier was trained on.\"\n        }\n      ]\n    },\n    \"Status\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the document classifier. If the status is <code>TRAINED</code> the classifier is ready to use. If the status is <code>TRAINED_WITH_WARNINGS</code> the classifier training succeeded, but you should review the warnings returned in the <code>CreateDocumentClassifier</code> response.</p> <p> If the status is <code>FAILED</code> you can see additional information about why the classifier wasn't trained in the <code>Message</code> field.</p>\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnyLengthString\"\n        },\n        {\n          \"description\": \"Additional information about the status of the classifier.\"\n        }\n      ]\n    },\n    \"SubmitTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n\
  \        },\n        {\n          \"description\": \"The time that the document classifier was submitted for training.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time that training the document classifier completed.\"\n        }\n      ]\n    },\n    \"TrainingStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Indicates the time when the training starts on documentation classifiers. You are billed for the time interval between this time and the value of TrainingEndTime. \"\n        }\n      ]\n    },\n    \"TrainingEndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time that training of the document classifier was completed. Indicates\
  \ the time when the training completes on documentation classifiers. You are billed for the time interval between this time and the value of TrainingStartTime.\"\n        }\n      ]\n    },\n    \"InputDataConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentClassifierInputDataConfig\"\n        },\n        {\n          \"description\": \"The input data configuration that you supplied when you created the document classifier for training.\"\n        }\n      ]\n    },\n    \"OutputDataConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentClassifierOutputDataConfig\"\n        },\n        {\n          \"description\": \" Provides output results configuration parameters for custom classifier jobs.\"\n        }\n      ]\n    },\n    \"ClassifierMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClassifierMetadata\"\n        },\n        {\n          \"description\": \"Information\
  \ about the document classifier, including the number of documents used for training the classifier, the number of documents used for test the classifier, and an accuracy rating.\"\n        }\n      ]\n    },\n    \"DataAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role that grants Amazon Comprehend read access to your input data.\"\n        }\n      ]\n    },\n    \"VolumeKmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyId\"\n        },\n        {\n          \"description\": \"<p>ID for the Amazon Web Services Key Management Service (KMS) key that Amazon Comprehend uses to encrypt data on the storage volume attached to the ML compute instance(s) that process the analysis job. The VolumeKmsKeyId can be either of the following formats:</p> <ul> <li> <p>KMS Key ID: <code>\\\"1234abcd-12ab-34cd-56ef-1234567890ab\\\
  \"</code> </p> </li> <li> <p>Amazon Resource Name (ARN) of a KMS Key: <code>\\\"arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab\\\"</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"VpcConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcConfig\"\n        },\n        {\n          \"description\": \" Configuration parameters for a private Virtual Private Cloud (VPC) containing the resources you are using for your custom classifier. For more information, see <a href=\\\"https://docs.aws.amazon.com/vppc/latest/userguide/what-is-amazon-vpc.html\\\">Amazon VPC</a>. \"\n        }\n      ]\n    },\n    \"Mode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentClassifierMode\"\n        },\n        {\n          \"description\": \"Indicates the mode in which the specific classifier was trained. This also indicates the format of input documents and the format of the confusion matrix. Each\
  \ classifier can only be trained in one mode and this cannot be changed once the classifier is trained.\"\n        }\n      ]\n    },\n    \"ModelKmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyId\"\n        },\n        {\n          \"description\": \"<p>ID for the KMS key that Amazon Comprehend uses to encrypt trained custom models. The ModelKmsKeyId can be either of the following formats:</p> <ul> <li> <p>KMS Key ID: <code>\\\"1234abcd-12ab-34cd-56ef-1234567890ab\\\"</code> </p> </li> <li> <p>Amazon Resource Name (ARN) of a KMS Key: <code>\\\"arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab\\\"</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"VersionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionName\"\n        },\n        {\n          \"description\": \"The version name that you assigned to the document classifier.\"\n        }\n      ]\n    },\n    \"SourceModelArn\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentClassifierArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the source model. This model was imported from a different Amazon Web Services account to create the document classifier model in your Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"FlywheelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendFlywheelArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of the flywheel\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-classifier-properties-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DocumentClassifierProperties
---
