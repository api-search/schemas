---
description: CreateDocumentClassifierRequest schema
layout: schema
name: CreateDocumentClassifierRequest
properties_list:
- description: ''
  name: DocumentClassifierName
  type: object
- description: ''
  name: VersionName
  type: object
- description: ''
  name: DataAccessRoleArn
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: InputDataConfig
  type: object
- description: ''
  name: OutputDataConfig
  type: object
- description: ''
  name: ClientRequestToken
  type: object
- description: ''
  name: LanguageCode
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
  name: ModelPolicy
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-create-document-classifier-request-schema.json
slug: openapi.yml-create-document-classifier-request
source_filename: openapi.yml-create-document-classifier-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-create-document-classifier-request-schema.json\",\n  \"title\": \"CreateDocumentClassifierRequest\",\n  \"description\": \"CreateDocumentClassifierRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DocumentClassifierName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendArnName\"\n        },\n        {\n          \"description\": \"The name of the document classifier.\"\n        }\n      ]\n    },\n    \"VersionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionName\"\n        },\n        {\n          \"description\": \"The version name given to the newly created classifier. Version names can have a maximum of 256 characters. Alphanumeric characters, hyphens (-) and underscores (_) are allowed.\
  \ The version name must be unique among all models with the same classifier name in the Amazon Web Services account/Amazon Web Services Region.\"\n        }\n      ]\n    },\n    \"DataAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role that grants Amazon Comprehend read access to your input data.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"Tags to associate with the document classifier. A tag is a key-value pair that adds as a metadata to a resource used by Amazon Comprehend. For example, a tag with \\\"Sales\\\" as the key might be added to a resource to indicate its use by the sales department. \"\n        }\n      ]\n    },\n    \"InputDataConfig\": {\n      \"allOf\": [\n        {\n       \
  \   \"$ref\": \"#/components/schemas/DocumentClassifierInputDataConfig\"\n        },\n        {\n          \"description\": \"Specifies the format and location of the input data for the job.\"\n        }\n      ]\n    },\n    \"OutputDataConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentClassifierOutputDataConfig\"\n        },\n        {\n          \"description\": \"Specifies the location for the output files from a custom classifier job. This parameter is required for a request that creates a native classifier model.\"\n        }\n      ]\n    },\n    \"ClientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestTokenString\"\n        },\n        {\n          \"description\": \"A unique identifier for the request. If you don't set the client request token, Amazon Comprehend generates one.\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/LanguageCode\"\n        },\n        {\n          \"description\": \"The language of the input documents. You can specify any of the languages supported by Amazon Comprehend. All documents must be in the same language.\"\n        }\n      ]\n    },\n    \"VolumeKmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyId\"\n        },\n        {\n          \"description\": \"<p>ID for the Amazon Web Services Key Management Service (KMS) key that Amazon Comprehend uses to encrypt data on the storage volume attached to the ML compute instance(s) that process the analysis job. The VolumeKmsKeyId can be either of the following formats:</p> <ul> <li> <p>KMS Key ID: <code>\\\"1234abcd-12ab-34cd-56ef-1234567890ab\\\"</code> </p> </li> <li> <p>Amazon Resource Name (ARN) of a KMS Key: <code>\\\"arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab\\\"</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"\
  VpcConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcConfig\"\n        },\n        {\n          \"description\": \"Configuration parameters for an optional private Virtual Private Cloud (VPC) containing the resources you are using for your custom classifier. For more information, see <a href=\\\"https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html\\\">Amazon VPC</a>. \"\n        }\n      ]\n    },\n    \"Mode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentClassifierMode\"\n        },\n        {\n          \"description\": \"Indicates the mode in which the classifier will be trained. The classifier can be trained in multi-class mode, which identifies one and only one class for each document, or multi-label mode, which identifies one or more labels for each document. In multi-label mode, multiple labels for an individual document are separated by a delimiter. The default delimiter between\
  \ labels is a pipe (|).\"\n        }\n      ]\n    },\n    \"ModelKmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyId\"\n        },\n        {\n          \"description\": \"<p>ID for the KMS key that Amazon Comprehend uses to encrypt trained custom models. The ModelKmsKeyId can be either of the following formats:</p> <ul> <li> <p>KMS Key ID: <code>\\\"1234abcd-12ab-34cd-56ef-1234567890ab\\\"</code> </p> </li> <li> <p>Amazon Resource Name (ARN) of a KMS Key: <code>\\\"arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab\\\"</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"ModelPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Policy\"\n        },\n        {\n          \"description\": \"<p>The resource-based policy to attach to your custom document classifier model. You can use this policy to allow another Amazon Web Services account to import your custom model.</p> <p>Provide\
  \ your policy as a JSON body that you enter as a UTF-8 encoded string without line breaks. To provide valid JSON, enclose the attribute names and values in double quotes. If the JSON body is also enclosed in double quotes, then you must escape the double quotes that are inside the policy:</p> <p> <code>\\\"{\\\\\\\"attribute\\\\\\\": \\\\\\\"value\\\\\\\", \\\\\\\"attribute\\\\\\\": [\\\\\\\"value\\\\\\\"]}\\\"</code> </p> <p>To avoid escaping quotes, you can use single quotes to enclose the policy and double quotes to enclose the JSON names and values:</p> <p> <code>'{\\\"attribute\\\": \\\"value\\\", \\\"attribute\\\": [\\\"value\\\"]}'</code> </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DocumentClassifierName\",\n    \"DataAccessRoleArn\",\n    \"InputDataConfig\",\n    \"LanguageCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-create-document-classifier-request-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: CreateDocumentClassifierRequest
---
