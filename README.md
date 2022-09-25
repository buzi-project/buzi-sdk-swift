# Swift5 API client for OpenAPIClient

This is a sample Pet Store Server based on the OpenAPI 3.0 specification.  You can find out more about
Swagger at [https://swagger.io](https://swagger.io). In the third iteration of the pet store, we've switched to the design first approach!
You can now help us improve the API whether it's by making changes to the definition itself or to the code.
That way, with time, we can improve the API in general, and expose some of the new features in OAS3.

_If you're looking for the Swagger 2.0/OAS 2.0 version of Petstore, then click [here](https://editor.swagger.io/?url=https://petstore.swagger.io/v2/swagger.yaml). Alternatively, you can load via the `Edit > Load Petstore OAS 2.0` menu option!_

Some useful links:
- [The Pet Store repository](https://github.com/swagger-api/swagger-petstore)
- [The source API definition for the Pet Store](https://github.com/swagger-api/swagger-petstore/blob/master/src/main/resources/openapi.yaml)

## Overview
This API client was generated by the [OpenAPI Generator](https://openapi-generator.tech) project.  By using the [openapi-spec](https://github.com/OAI/OpenAPI-Specification) from a remote server, you can easily generate an API client.

- API version: 1.0.0
- Package version: 
- Build package: org.openapitools.codegen.languages.Swift5ClientCodegen

## Installation

### Carthage

Run `carthage update`

### CocoaPods

Run `pod install`

## Documentation for API Endpoints

All URIs are relative to *https://petstore3.swagger.io*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*SmsAPI* | [**cancelMessage**](docs/SmsAPI.md#cancelmessage) | **POST** /v1/sms/messages/{messageId}/cancel | Cancel a message
*SmsAPI* | [**createMessage**](docs/SmsAPI.md#createmessage) | **POST** /v1/sms/messages | Create Message
*SmsAPI* | [**createPricing**](docs/SmsAPI.md#createpricing) | **PUT** /v1/sms/networks/{networkId}/pricing | Create network price
*SmsAPI* | [**deleteMessage**](docs/SmsAPI.md#deletemessage) | **DELETE** /v1/sms/messages/{messageId} | Deletes a message
*SmsAPI* | [**getMessage**](docs/SmsAPI.md#getmessage) | **GET** /v1/sms/messages/{messageId} | Get message
*SmsAPI* | [**getNetwork**](docs/SmsAPI.md#getnetwork) | **GET** /v1/sms/networks/{networkId} | Get network
*SmsAPI* | [**getPricing**](docs/SmsAPI.md#getpricing) | **GET** /v1/sms/networks/{networkId}/pricing | List network rates
*SmsAPI* | [**listMessages**](docs/SmsAPI.md#listmessages) | **GET** /v1/sms/messages | List messages
*SmsAPI* | [**listNetworks**](docs/SmsAPI.md#listnetworks) | **GET** /v1/sms/networks | List networks
*SmsAPI* | [**sendMessage**](docs/SmsAPI.md#sendmessage) | **POST** /v1/sms/messages/{messageId}/send | Sends a message


## Documentation For Models

 - [Cost](docs/Cost.md)
 - [CreateMessageInput](docs/CreateMessageInput.md)
 - [Message](docs/Message.md)
 - [ModelError](docs/ModelError.md)
 - [Network](docs/Network.md)
 - [Pricing](docs/Pricing.md)


## Documentation For Authorization


## ApiKeyAuth

- **Type**: API key
- **API key parameter name**: X-API-Key
- **Location**: HTTP header

## BasicAuth

- **Type**: HTTP basic authentication

## BearerAuth

- **Type**: HTTP basic authentication


## Author

edson@michaque.com

