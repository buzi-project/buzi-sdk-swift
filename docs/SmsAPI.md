# SmsAPI

All URIs are relative to *https://petstore3.swagger.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancelMessage**](SmsAPI.md#cancelmessage) | **POST** /v1/sms/messages/{messageId}/cancel | Cancel a message
[**createMessage**](SmsAPI.md#createmessage) | **POST** /v1/sms/messages | Create Message
[**createPricing**](SmsAPI.md#createpricing) | **PUT** /v1/sms/networks/{networkId}/pricing | Create network price
[**deleteMessage**](SmsAPI.md#deletemessage) | **DELETE** /v1/sms/messages/{messageId} | Deletes a message
[**getMessage**](SmsAPI.md#getmessage) | **GET** /v1/sms/messages/{messageId} | Get message
[**getNetwork**](SmsAPI.md#getnetwork) | **GET** /v1/sms/networks/{networkId} | Get network
[**getPricing**](SmsAPI.md#getpricing) | **GET** /v1/sms/networks/{networkId}/pricing | List network rates
[**listMessages**](SmsAPI.md#listmessages) | **GET** /v1/sms/messages | List messages
[**listNetworks**](SmsAPI.md#listnetworks) | **GET** /v1/sms/networks | List networks
[**sendMessage**](SmsAPI.md#sendmessage) | **POST** /v1/sms/messages/{messageId}/send | Sends a message


# **cancelMessage**
```swift
    open class func cancelMessage(messageId: Int64, completion: @escaping (_ data: Message?, _ error: Error?) -> Void)
```

Cancel a message

Returns a single pet

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let messageId = 987 // Int64 | ID of pet to return

// Cancel a message
SmsAPI.cancelMessage(messageId: messageId) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **messageId** | **Int64** | ID of pet to return | 

### Return type

[**Message**](Message.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createMessage**
```swift
    open class func createMessage(createMessageInput: CreateMessageInput, completion: @escaping (_ data: Message?, _ error: Error?) -> Void)
```

Create Message

Update an existing pet by Id

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let createMessageInput = CreateMessageInput(to: ["to_example"], from: "from_example", networkId: 123, callbackUrl: "callbackUrl_example") // CreateMessageInput | Update an existent pet in the store

// Create Message
SmsAPI.createMessage(createMessageInput: createMessageInput) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createMessageInput** | [**CreateMessageInput**](CreateMessageInput.md) | Update an existent pet in the store | 

### Return type

[**Message**](Message.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createPricing**
```swift
    open class func createPricing(networkId: Int, completion: @escaping (_ data: Message?, _ error: Error?) -> Void)
```

Create network price

Returns a single pet

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let networkId = 987 // Int | 

// Create network price
SmsAPI.createPricing(networkId: networkId) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **networkId** | **Int** |  | 

### Return type

[**Message**](Message.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteMessage**
```swift
    open class func deleteMessage(messageId: Int64, apiKey: String? = nil, completion: @escaping (_ data: ModelError?, _ error: Error?) -> Void)
```

Deletes a message

delete a message

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let messageId = 987 // Int64 | Pet id to delete
let apiKey = "apiKey_example" // String |  (optional)

// Deletes a message
SmsAPI.deleteMessage(messageId: messageId, apiKey: apiKey) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **messageId** | **Int64** | Pet id to delete | 
 **apiKey** | **String** |  | [optional] 

### Return type

[**ModelError**](ModelError.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getMessage**
```swift
    open class func getMessage(messageId: Int64, completion: @escaping (_ data: Message?, _ error: Error?) -> Void)
```

Get message

Returns a single pet

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let messageId = 987 // Int64 | ID of pet to return

// Get message
SmsAPI.getMessage(messageId: messageId) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **messageId** | **Int64** | ID of pet to return | 

### Return type

[**Message**](Message.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getNetwork**
```swift
    open class func getNetwork(networkId: Int, countryCode: Int64? = nil, completion: @escaping (_ data: Network?, _ error: Error?) -> Void)
```

Get network

Returns a single pet

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let networkId = 987 // Int | 
let countryCode = 987 // Int64 | ID of pet to return (optional)

// Get network
SmsAPI.getNetwork(networkId: networkId, countryCode: countryCode) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **networkId** | **Int** |  | 
 **countryCode** | **Int64** | ID of pet to return | [optional] 

### Return type

[**Network**](Network.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getPricing**
```swift
    open class func getPricing(networkId: Int, completion: @escaping (_ data: [Pricing]?, _ error: Error?) -> Void)
```

List network rates

Returns a single pet

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let networkId = 987 // Int | 

// List network rates
SmsAPI.getPricing(networkId: networkId) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **networkId** | **Int** |  | 

### Return type

[**[Pricing]**](Pricing.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **listMessages**
```swift
    open class func listMessages(inbox: String? = nil, status: String? = nil, completion: @escaping (_ data: [Message]?, _ error: Error?) -> Void)
```

List messages

Update an existing pet by Id

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let inbox = "inbox_example" // String |  (optional)
let status = "status_example" // String |  (optional)

// List messages
SmsAPI.listMessages(inbox: inbox, status: status) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inbox** | **String** |  | [optional] 
 **status** | **String** |  | [optional] 

### Return type

[**[Message]**](Message.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **listNetworks**
```swift
    open class func listNetworks(countryCode: String? = nil, completion: @escaping (_ data: [Network]?, _ error: Error?) -> Void)
```

List networks

Returns a single pet

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let countryCode = "countryCode_example" // String | ID of pet to return (optional)

// List networks
SmsAPI.listNetworks(countryCode: countryCode) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **countryCode** | **String** | ID of pet to return | [optional] 

### Return type

[**[Network]**](Network.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **sendMessage**
```swift
    open class func sendMessage(messageId: Int64, completion: @escaping (_ data: Message?, _ error: Error?) -> Void)
```

Sends a message

Returns a single pet

### Example
```swift
// The following code samples are still beta. For any issue, please report via http://github.com/OpenAPITools/openapi-generator/issues/new
import OpenAPIClient

let messageId = 987 // Int64 | ID of pet to return

// Sends a message
SmsAPI.sendMessage(messageId: messageId) { (response, error) in
    guard error == nil else {
        print(error)
        return
    }

    if (response) {
        dump(response)
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **messageId** | **Int64** | ID of pet to return | 

### Return type

[**Message**](Message.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BasicAuth](../README.md#BasicAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

