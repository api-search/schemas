---
description: Represents the request to create a user pool client.
layout: schema
name: CreateUserPoolClientRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: ClientName
  type: object
- description: ''
  name: GenerateSecret
  type: object
- description: ''
  name: RefreshTokenValidity
  type: object
- description: ''
  name: AccessTokenValidity
  type: object
- description: ''
  name: IdTokenValidity
  type: object
- description: ''
  name: TokenValidityUnits
  type: object
- description: ''
  name: ReadAttributes
  type: object
- description: ''
  name: WriteAttributes
  type: object
- description: ''
  name: ExplicitAuthFlows
  type: object
- description: ''
  name: SupportedIdentityProviders
  type: object
- description: ''
  name: CallbackURLs
  type: object
- description: ''
  name: LogoutURLs
  type: object
- description: ''
  name: DefaultRedirectURI
  type: object
- description: ''
  name: AllowedOAuthFlows
  type: object
- description: ''
  name: AllowedOAuthScopes
  type: object
- description: ''
  name: AllowedOAuthFlowsUserPoolClient
  type: object
- description: ''
  name: AnalyticsConfiguration
  type: object
- description: ''
  name: PreventUserExistenceErrors
  type: object
- description: ''
  name: EnableTokenRevocation
  type: object
- description: ''
  name: EnablePropagateAdditionalUserContextData
  type: object
- description: ''
  name: AuthSessionValidity
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-create-user-pool-client-request-schema.json
slug: user-pools-create-user-pool-client-request
source_filename: user-pools-create-user-pool-client-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-create-user-pool-client-request-schema.json\",\n  \"title\": \"CreateUserPoolClientRequest\",\n  \"description\": \"Represents the request to create a user pool client.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool where you want to create a user pool client.\"\n        }\n      ]\n    },\n    \"ClientName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientNameType\"\n        },\n        {\n          \"description\": \"The client name for the user pool client you would like to create.\"\n        }\n      ]\n    },\n    \"GenerateSecret\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/GenerateSecret\"\n        },\n        {\n          \"description\": \"Boolean to specify whether you want to generate a secret for the user pool client being created.\"\n        }\n      ]\n    },\n    \"RefreshTokenValidity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RefreshTokenValidityType\"\n        },\n        {\n          \"description\": \"<p>The refresh token time limit. After this limit expires, your user can't use their refresh token. To specify the time unit for <code>RefreshTokenValidity</code> as <code>seconds</code>, <code>minutes</code>, <code>hours</code>, or <code>days</code>, set a <code>TokenValidityUnits</code> value in your API request.</p> <p>For example, when you set <code>RefreshTokenValidity</code> as <code>10</code> and <code>TokenValidityUnits</code> as <code>days</code>, your user can refresh their session and retrieve new access and ID tokens for 10 days.</p> <p>The\
  \ default time unit for <code>RefreshTokenValidity</code> in an API request is days. You can't set <code>RefreshTokenValidity</code> to 0. If you do, Amazon Cognito overrides the value with the default value of 30 days. <i>Valid range</i> is displayed below in seconds.</p> <p>If you don't specify otherwise in the configuration of your app client, your refresh tokens are valid for 30 days.</p>\"\n        }\n      ]\n    },\n    \"AccessTokenValidity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessTokenValidityType\"\n        },\n        {\n          \"description\": \"<p>The access token time limit. After this limit expires, your user can't use their access token. To specify the time unit for <code>AccessTokenValidity</code> as <code>seconds</code>, <code>minutes</code>, <code>hours</code>, or <code>days</code>, set a <code>TokenValidityUnits</code> value in your API request.</p> <p>For example, when you set <code>AccessTokenValidity</code> to <code>10</code>\
  \ and <code>TokenValidityUnits</code> to <code>hours</code>, your user can authorize access with their access token for 10 hours.</p> <p>The default time unit for <code>AccessTokenValidity</code> in an API request is hours. <i>Valid range</i> is displayed below in seconds.</p> <p>If you don't specify otherwise in the configuration of your app client, your access tokens are valid for one hour.</p>\"\n        }\n      ]\n    },\n    \"IdTokenValidity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdTokenValidityType\"\n        },\n        {\n          \"description\": \"<p>The ID token time limit. After this limit expires, your user can't use their ID token. To specify the time unit for <code>IdTokenValidity</code> as <code>seconds</code>, <code>minutes</code>, <code>hours</code>, or <code>days</code>, set a <code>TokenValidityUnits</code> value in your API request.</p> <p>For example, when you set <code>IdTokenValidity</code> as <code>10</code> and <code>TokenValidityUnits</code>\
  \ as <code>hours</code>, your user can authenticate their session with their ID token for 10 hours.</p> <p>The default time unit for <code>IdTokenValidity</code> in an API request is hours. <i>Valid range</i> is displayed below in seconds.</p> <p>If you don't specify otherwise in the configuration of your app client, your ID tokens are valid for one hour.</p>\"\n        }\n      ]\n    },\n    \"TokenValidityUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenValidityUnitsType\"\n        },\n        {\n          \"description\": \"The units in which the validity times are represented. The default unit for RefreshToken is days, and default for ID and access tokens are hours.\"\n        }\n      ]\n    },\n    \"ReadAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientPermissionListType\"\n        },\n        {\n          \"description\": \"The read attributes.\"\n        }\n      ]\n    },\n    \"WriteAttributes\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientPermissionListType\"\n        },\n        {\n          \"description\": \"<p>The user pool attributes that the app client can write to.</p> <p>If your app client allows users to sign in through an IdP, this array must include all attributes that you have mapped to IdP attributes. Amazon Cognito updates mapped attributes when users sign in to your application through an IdP. If your app client does not have write access to a mapped attribute, Amazon Cognito throws an error when it tries to update the attribute. For more information, see <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pools-specifying-attribute-mapping.html\\\">Specifying IdP Attribute Mappings for Your user pool</a>.</p>\"\n        }\n      ]\n    },\n    \"ExplicitAuthFlows\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExplicitAuthFlowsListType\"\n        },\n       \
  \ {\n          \"description\": \"<p>The authentication flows that you want your user pool client to support. For each app client in your user pool, you can sign in your users with any combination of one or more flows, including with a user name and Secure Remote Password (SRP), a user name and password, or a custom authentication process that you define with Lambda functions.</p> <note> <p>If you don't specify a value for <code>ExplicitAuthFlows</code>, your user client supports <code>ALLOW_REFRESH_TOKEN_AUTH</code>, <code>ALLOW_USER_SRP_AUTH</code>, and <code>ALLOW_CUSTOM_AUTH</code>.</p> </note> <p>Valid values include:</p> <ul> <li> <p> <code>ALLOW_ADMIN_USER_PASSWORD_AUTH</code>: Enable admin based user password authentication flow <code>ADMIN_USER_PASSWORD_AUTH</code>. This setting replaces the <code>ADMIN_NO_SRP_AUTH</code> setting. With this authentication flow, your app passes a user name and password to Amazon Cognito in the request, instead of using the Secure Remote Password\
  \ (SRP) protocol to securely transmit the password.</p> </li> <li> <p> <code>ALLOW_CUSTOM_AUTH</code>: Enable Lambda trigger based authentication.</p> </li> <li> <p> <code>ALLOW_USER_PASSWORD_AUTH</code>: Enable user password-based authentication. In this flow, Amazon Cognito receives the password in the request instead of using the SRP protocol to verify passwords.</p> </li> <li> <p> <code>ALLOW_USER_SRP_AUTH</code>: Enable SRP-based authentication.</p> </li> <li> <p> <code>ALLOW_REFRESH_TOKEN_AUTH</code>: Enable authflow to refresh tokens.</p> </li> </ul> <p>In some environments, you will see the values <code>ADMIN_NO_SRP_AUTH</code>, <code>CUSTOM_AUTH_FLOW_ONLY</code>, or <code>USER_PASSWORD_AUTH</code>. You can't assign these legacy <code>ExplicitAuthFlows</code> values to user pool clients at the same time as values that begin with <code>ALLOW_</code>, like <code>ALLOW_USER_SRP_AUTH</code>.</p>\"\n        }\n      ]\n    },\n    \"SupportedIdentityProviders\": {\n      \"allOf\":\
  \ [\n        {\n          \"$ref\": \"#/components/schemas/SupportedIdentityProvidersListType\"\n        },\n        {\n          \"description\": \"A list of provider names for the identity providers (IdPs) that are supported on this client. The following are supported: <code>COGNITO</code>, <code>Facebook</code>, <code>Google</code>, <code>SignInWithApple</code>, and <code>LoginWithAmazon</code>. You can also specify the names that you configured for the SAML and OIDC IdPs in your user pool, for example <code>MySAMLIdP</code> or <code>MyOIDCIdP</code>.\"\n        }\n      ]\n    },\n    \"CallbackURLs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CallbackURLsListType\"\n        },\n        {\n          \"description\": \"<p>A list of allowed redirect (callback) URLs for the IdPs.</p> <p>A redirect URI must:</p> <ul> <li> <p>Be an absolute URI.</p> </li> <li> <p>Be registered with the authorization server.</p> </li> <li> <p>Not include a fragment component.</p>\
  \ </li> </ul> <p>See <a href=\\\"https://tools.ietf.org/html/rfc6749#section-3.1.2\\\">OAuth 2.0 - Redirection Endpoint</a>.</p> <p>Amazon Cognito requires HTTPS over HTTP except for http://localhost for testing purposes only.</p> <p>App callback URLs such as myapp://example are also supported.</p>\"\n        }\n      ]\n    },\n    \"LogoutURLs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogoutURLsListType\"\n        },\n        {\n          \"description\": \"A list of allowed logout URLs for the IdPs.\"\n        }\n      ]\n    },\n    \"DefaultRedirectURI\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RedirectUrlType\"\n        },\n        {\n          \"description\": \"<p>The default redirect URI. Must be in the <code>CallbackURLs</code> list.</p> <p>A redirect URI must:</p> <ul> <li> <p>Be an absolute URI.</p> </li> <li> <p>Be registered with the authorization server.</p> </li> <li> <p>Not include a fragment component.</p>\
  \ </li> </ul> <p>See <a href=\\\"https://tools.ietf.org/html/rfc6749#section-3.1.2\\\">OAuth 2.0 - Redirection Endpoint</a>.</p> <p>Amazon Cognito requires HTTPS over HTTP except for http://localhost for testing purposes only.</p> <p>App callback URLs such as myapp://example are also supported.</p>\"\n        }\n      ]\n    },\n    \"AllowedOAuthFlows\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OAuthFlowsType\"\n        },\n        {\n          \"description\": \"<p>The allowed OAuth flows.</p> <dl> <dt>code</dt> <dd> <p>Use a code grant flow, which provides an authorization code as the response. This code can be exchanged for access tokens with the <code>/oauth2/token</code> endpoint.</p> </dd> <dt>implicit</dt> <dd> <p>Issue the access token (and, optionally, ID token, based on scopes) directly to your user.</p> </dd> <dt>client_credentials</dt> <dd> <p>Issue the access token from the <code>/oauth2/token</code> endpoint directly to a non-person user\
  \ using a combination of the client ID and client secret.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"AllowedOAuthScopes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScopeListType\"\n        },\n        {\n          \"description\": \"The allowed OAuth scopes. Possible values provided by OAuth are <code>phone</code>, <code>email</code>, <code>openid</code>, and <code>profile</code>. Possible values provided by Amazon Web Services are <code>aws.cognito.signin.user.admin</code>. Custom scopes created in Resource Servers are also supported.\"\n        }\n      ]\n    },\n    \"AllowedOAuthFlowsUserPoolClient\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanType\"\n        },\n        {\n          \"description\": \"<p>Set to <code>true</code> to use OAuth 2.0 features in your user pool app client.</p> <p> <code>AllowedOAuthFlowsUserPoolClient</code> must be <code>true</code> before you can configure the following\
  \ features in your app client.</p> <ul> <li> <p> <code>CallBackURLs</code>: Callback URLs.</p> </li> <li> <p> <code>LogoutURLs</code>: Sign-out redirect URLs.</p> </li> <li> <p> <code>AllowedOAuthScopes</code>: OAuth 2.0 scopes.</p> </li> <li> <p> <code>AllowedOAuthFlows</code>: Support for authorization code, implicit, and client credentials OAuth 2.0 grants.</p> </li> </ul> <p>To use OAuth 2.0 features, configure one of these features in the Amazon Cognito console or set <code>AllowedOAuthFlowsUserPoolClient</code> to <code>true</code> in a <code>CreateUserPoolClient</code> or <code>UpdateUserPoolClient</code> API request. If you don't set a value for <code>AllowedOAuthFlowsUserPoolClient</code> in a request with the CLI or SDKs, it defaults to <code>false</code>.</p>\"\n        }\n      ]\n    },\n    \"AnalyticsConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalyticsConfigurationType\"\n        },\n        {\n          \"description\"\
  : \"<p>The user pool analytics configuration for collecting metrics and sending them to your Amazon Pinpoint campaign.</p> <note> <p>In Amazon Web Services Regions where Amazon Pinpoint isn't available, user pools only support sending events to Amazon Pinpoint projects in Amazon Web Services Region us-east-1. In Regions where Amazon Pinpoint is available, user pools support sending events to Amazon Pinpoint projects within that same Region.</p> </note>\"\n        }\n      ]\n    },\n    \"PreventUserExistenceErrors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PreventUserExistenceErrorTypes\"\n        },\n        {\n          \"description\": \"<p>Errors and responses that you want Amazon Cognito APIs to return during authentication, account confirmation, and password recovery when the user doesn't exist in the user pool. When set to <code>ENABLED</code> and the user doesn't exist, authentication returns an error indicating either the username or password\
  \ was incorrect. Account confirmation and password recovery return a response indicating a code was sent to a simulated destination. When set to <code>LEGACY</code>, those APIs return a <code>UserNotFoundException</code> exception if the user doesn't exist in the user pool.</p> <p>Valid values include:</p> <ul> <li> <p> <code>ENABLED</code> - This prevents user existence-related errors.</p> </li> <li> <p> <code>LEGACY</code> - This represents the early behavior of Amazon Cognito where user existence related errors aren't prevented.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"EnableTokenRevocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrappedBooleanType\"\n        },\n        {\n          \"description\": \"<p>Activates or deactivates token revocation. For more information about revoking tokens, see <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_RevokeToken.html\\\">RevokeToken</a>.</p> <p>If\
  \ you don't include this parameter, token revocation is automatically activated for the new user pool client.</p>\"\n        }\n      ]\n    },\n    \"EnablePropagateAdditionalUserContextData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrappedBooleanType\"\n        },\n        {\n          \"description\": \"Activates the propagation of additional user context data. For more information about propagation of user context data, see <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pool-settings-advanced-security.html\\\"> Adding advanced security to a user pool</a>. If you don\\u2019t include this parameter, you can't send device fingerprint information, including source IP address, to Amazon Cognito advanced security. You can only activate <code>EnablePropagateAdditionalUserContextData</code> in an app client that has a client secret.\"\n        }\n      ]\n    },\n    \"AuthSessionValidity\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/AuthSessionValidityType\"\n        },\n        {\n          \"description\": \"Amazon Cognito creates a session token for each API request in an authentication flow. <code>AuthSessionValidity</code> is the duration, in minutes, of that session token. Your user pool native user must respond to each authentication challenge before the session expires.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"ClientName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-create-user-pool-client-request-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: CreateUserPoolClientRequest
---
