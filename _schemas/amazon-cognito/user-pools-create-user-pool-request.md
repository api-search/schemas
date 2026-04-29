---
description: Represents the request to create a user pool.
layout: schema
name: CreateUserPoolRequest
properties_list:
- description: ''
  name: PoolName
  type: object
- description: ''
  name: Policies
  type: object
- description: ''
  name: DeletionProtection
  type: object
- description: ''
  name: LambdaConfig
  type: object
- description: ''
  name: AutoVerifiedAttributes
  type: object
- description: ''
  name: AliasAttributes
  type: object
- description: ''
  name: UsernameAttributes
  type: object
- description: ''
  name: SmsVerificationMessage
  type: object
- description: ''
  name: EmailVerificationMessage
  type: object
- description: ''
  name: EmailVerificationSubject
  type: object
- description: ''
  name: VerificationMessageTemplate
  type: object
- description: ''
  name: SmsAuthenticationMessage
  type: object
- description: ''
  name: MfaConfiguration
  type: object
- description: ''
  name: UserAttributeUpdateSettings
  type: object
- description: ''
  name: DeviceConfiguration
  type: object
- description: ''
  name: EmailConfiguration
  type: object
- description: ''
  name: SmsConfiguration
  type: object
- description: ''
  name: UserPoolTags
  type: object
- description: ''
  name: AdminCreateUserConfig
  type: object
- description: ''
  name: Schema
  type: object
- description: ''
  name: UserPoolAddOns
  type: object
- description: ''
  name: UsernameConfiguration
  type: object
- description: ''
  name: AccountRecoverySetting
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-create-user-pool-request-schema.json
slug: user-pools-create-user-pool-request
source_filename: user-pools-create-user-pool-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-create-user-pool-request-schema.json\",\n  \"title\": \"CreateUserPoolRequest\",\n  \"description\": \"Represents the request to create a user pool.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PoolName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolNameType\"\n        },\n        {\n          \"description\": \"A string used to name the user pool.\"\n        }\n      ]\n    },\n    \"Policies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolPolicyType\"\n        },\n        {\n          \"description\": \"The policies associated with the new user pool.\"\n        }\n      ]\n    },\n    \"DeletionProtection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeletionProtectionType\"\
  \n        },\n        {\n          \"description\": \"<p>When active, <code>DeletionProtection</code> prevents accidental deletion of your user pool. Before you can delete a user pool that you have protected against deletion, you must deactivate this feature.</p> <p>When you try to delete a protected user pool in a <code>DeleteUserPool</code> API request, Amazon Cognito returns an <code>InvalidParameterException</code> error. To delete a protected user pool, send a new <code>DeleteUserPool</code> request after you deactivate deletion protection in an <code>UpdateUserPool</code> API request.</p>\"\n        }\n      ]\n    },\n    \"LambdaConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaConfigType\"\n        },\n        {\n          \"description\": \"<p>The Lambda trigger configuration information for the new user pool.</p> <note> <p>In a push model, event sources (such as Amazon S3 and custom applications) need permission to invoke a function.\
  \ So you must make an extra call to add permission for these event sources to invoke your Lambda function.</p> <p/> <p>For more information on using the Lambda API to add permission, see<a href=\\\"https://docs.aws.amazon.com/lambda/latest/dg/API_AddPermission.html\\\"> AddPermission </a>. </p> <p>For adding permission using the CLI, see<a href=\\\"https://docs.aws.amazon.com/cli/latest/reference/lambda/add-permission.html\\\"> add-permission </a>.</p> </note>\"\n        }\n      ]\n    },\n    \"AutoVerifiedAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VerifiedAttributesListType\"\n        },\n        {\n          \"description\": \"The attributes to be auto-verified. Possible values: <b>email</b>, <b>phone_number</b>.\"\n        }\n      ]\n    },\n    \"AliasAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AliasAttributesListType\"\n        },\n        {\n          \"description\": \"Attributes supported\
  \ as an alias for this user pool. Possible values: <b>phone_number</b>, <b>email</b>, or <b>preferred_username</b>.\"\n        }\n      ]\n    },\n    \"UsernameAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsernameAttributesListType\"\n        },\n        {\n          \"description\": \"Specifies whether a user can use an email address or phone number as a username when they sign up.\"\n        }\n      ]\n    },\n    \"SmsVerificationMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmsVerificationMessageType\"\n        },\n        {\n          \"description\": \"This parameter is no longer used. See <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_VerificationMessageTemplateType.html\\\">VerificationMessageTemplateType</a>.\"\n        }\n      ]\n    },\n    \"EmailVerificationMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailVerificationMessageType\"\
  \n        },\n        {\n          \"description\": \"This parameter is no longer used. See <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_VerificationMessageTemplateType.html\\\">VerificationMessageTemplateType</a>.\"\n        }\n      ]\n    },\n    \"EmailVerificationSubject\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailVerificationSubjectType\"\n        },\n        {\n          \"description\": \"This parameter is no longer used. See <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_VerificationMessageTemplateType.html\\\">VerificationMessageTemplateType</a>.\"\n        }\n      ]\n    },\n    \"VerificationMessageTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VerificationMessageTemplateType\"\n        },\n        {\n          \"description\": \"The template for the verification message that the user sees when the app\
  \ requests permission to access the user's information.\"\n        }\n      ]\n    },\n    \"SmsAuthenticationMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmsVerificationMessageType\"\n        },\n        {\n          \"description\": \"A string representing the SMS authentication message.\"\n        }\n      ]\n    },\n    \"MfaConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolMfaType\"\n        },\n        {\n          \"description\": \"Specifies MFA configuration details.\"\n        }\n      ]\n    },\n    \"UserAttributeUpdateSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserAttributeUpdateSettingsType\"\n        },\n        {\n          \"description\": \"The settings for updates to user attributes. These settings include the property <code>AttributesRequireVerificationBeforeUpdate</code>, a user-pool setting that tells Amazon Cognito how to handle\
  \ changes to the value of your users' email address and phone number attributes. For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/user-pool-settings-email-phone-verification.html#user-pool-settings-verifications-verify-attribute-updates\\\"> Verifying updates to email addresses and phone numbers</a>.\"\n        }\n      ]\n    },\n    \"DeviceConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceConfigurationType\"\n        },\n        {\n          \"description\": \"<p>The device-remembering configuration for a user pool. A null value indicates that you have deactivated device remembering in your user pool.</p> <note> <p>When you provide a value for any <code>DeviceConfiguration</code> field, you activate the Amazon Cognito device-remembering feature.</p> </note>\"\n        }\n      ]\n    },\n    \"EmailConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailConfigurationType\"\
  \n        },\n        {\n          \"description\": \"The email configuration of your user pool. The email configuration type sets your preferred sending method, Amazon Web Services Region, and sender for messages from your user pool.\"\n        }\n      ]\n    },\n    \"SmsConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmsConfigurationType\"\n        },\n        {\n          \"description\": \"The SMS configuration with the settings that your Amazon Cognito user pool must use to send an SMS message from your Amazon Web Services account through Amazon Simple Notification Service. To send SMS messages with Amazon SNS in the Amazon Web Services Region that you want, the Amazon Cognito user pool uses an Identity and Access Management (IAM) role in your Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"UserPoolTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolTagsType\"\n        },\n \
  \       {\n          \"description\": \"The tag keys and values to assign to the user pool. A tag is a label that you can use to categorize and manage user pools in different ways, such as by purpose, owner, environment, or other criteria.\"\n        }\n      ]\n    },\n    \"AdminCreateUserConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdminCreateUserConfigType\"\n        },\n        {\n          \"description\": \"The configuration for <code>AdminCreateUser</code> requests.\"\n        }\n      ]\n    },\n    \"Schema\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SchemaAttributesListType\"\n        },\n        {\n          \"description\": \"An array of schema attributes for the new user pool. These attributes can be standard or custom attributes.\"\n        }\n      ]\n    },\n    \"UserPoolAddOns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolAddOnsType\"\n        },\n\
  \        {\n          \"description\": \"<p>User pool add-ons. Contains settings for activation of advanced security features. To log user security information but take no action, set to <code>AUDIT</code>. To configure automatic security responses to risky traffic to your user pool, set to <code>ENFORCED</code>.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pool-settings-advanced-security.html\\\">Adding advanced security to a user pool</a>.</p>\"\n        }\n      ]\n    },\n    \"UsernameConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsernameConfigurationType\"\n        },\n        {\n          \"description\": \"<p>Case sensitivity on the username input for the selected sign-in option. When case sensitivity is set to <code>False</code> (case insensitive), users can sign in with any combination of capital and lowercase letters. For example, <code>username</code>, <code>USERNAME</code>,\
  \ or <code>UserName</code>, or for email, <code>email@example.com</code> or <code>EMaiL@eXamplE.Com</code>. For most use cases, set case sensitivity to <code>False</code> (case insensitive) as a best practice. When usernames and email addresses are case insensitive, Amazon Cognito treats any variation in case as the same user, and prevents a case variation from being assigned to the same attribute for a different user.</p> <p>This configuration is immutable after you set it. For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_UsernameConfigurationType.html\\\">UsernameConfigurationType</a>.</p>\"\n        }\n      ]\n    },\n    \"AccountRecoverySetting\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountRecoverySettingType\"\n        },\n        {\n          \"description\": \"The available verified method a user can use to recover their password when they call <code>ForgotPassword</code>.\
  \ You can use this setting to define a preferred method when a user has more than one method available. With this setting, SMS doesn't qualify for a valid password recovery mechanism if the user also has SMS multi-factor authentication (MFA) activated. In the absence of this setting, Amazon Cognito uses the legacy behavior to determine the recovery method where SMS is preferred through email.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PoolName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-create-user-pool-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: CreateUserPoolRequest
---
