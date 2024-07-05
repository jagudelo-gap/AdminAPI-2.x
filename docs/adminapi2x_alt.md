# Admin API Documentation
## Version: v2

### /v2/resourceClaims

#### GET
##### Summary:

Retrieves all resourceClaims.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| offset | query | Indicates how many items should be skipped before returning results. | Yes | integer |
| limit | query | Indicates the maximum number of items that should be returned in the results. | Yes | integer |
| sortBy | query |  | No | string |
| descendingSorting | query |  | No | boolean |
| id | query | Resource Claim Id | No | integer |
| name | query | Resource Claim Name | No | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/resourceClaims/{id}

#### GET
##### Summary:

Retrieves a specific resourceClaim based on the identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/vendors

#### GET
##### Summary:

Retrieves all vendors.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| offset | query | Indicates how many items should be skipped before returning results. | Yes | integer |
| limit | query | Indicates the maximum number of items that should be returned in the results. | Yes | integer |
| sortBy | query |  | No | string |
| descendingSorting | query |  | No | boolean |
| id | query | Vendor/ company id | No | integer |
| company | query | Vendor/ company name | No | string |
| namespacePrefixes | query | Namespace prefix for the vendor. Multiple namespace prefixes can be provided as comma separated list if required. | No | string |
| contactName | query | Vendor contact name | No | string |
| contactEmailAddress | query | Vendor contact email id | No | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### POST
##### Summary:

Creates vendor based on the supplied values.

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Created |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/vendors/{id}

#### GET
##### Summary:

Retrieves a specific vendor based on the identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### PUT
##### Summary:

Updates vendor based on the resource identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### DELETE
##### Summary:

Deletes an existing vendor using the resource identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Resource was successfully deleted. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/profiles

#### GET
##### Summary:

Retrieves all profiles.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| offset | query | Indicates how many items should be skipped before returning results. | Yes | integer |
| limit | query | Indicates the maximum number of items that should be returned in the results. | Yes | integer |
| sortBy | query |  | No | string |
| descendingSorting | query |  | No | boolean |
| id | query | Profile id | No | integer |
| name | query | Profile name | No | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### POST
##### Summary:

Creates profile based on the supplied values.

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Created |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/profiles/{id}

#### GET
##### Summary:

Retrieves a specific profile based on the identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### PUT
##### Summary:

Updates profile based on the resource identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### DELETE
##### Summary:

Deletes an existing profile using the resource identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Resource was successfully deleted. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/odsInstances

#### GET
##### Summary:

Retrieves all odsInstances.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| offset | query | Indicates how many items should be skipped before returning results. | Yes | integer |
| limit | query | Indicates the maximum number of items that should be returned in the results. | Yes | integer |
| sortBy | query |  | No | string |
| descendingSorting | query |  | No | boolean |
| id | query | List of ODS instance id | No | integer |
| name | query | Ods Instance name | No | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### POST
##### Summary:

Creates odsInstance based on the supplied values.

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Created |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/odsInstances/{id}

#### GET
##### Summary:

Retrieves a specific odsInstance based on the identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### PUT
##### Summary:

Updates odsInstance based on the resource identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### DELETE
##### Summary:

Deletes an existing odsInstance using the resource identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Resource was successfully deleted. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/odsInstanceDerivatives

#### GET
##### Summary:

Retrieves all odsInstanceDerivatives.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| offset | query | Indicates how many items should be skipped before returning results. | Yes | integer |
| limit | query | Indicates the maximum number of items that should be returned in the results. | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### POST
##### Summary:

Creates odsInstanceDerivative based on the supplied values.

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Created |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/odsInstanceDerivatives/{id}

#### GET
##### Summary:

Retrieves a specific odsInstanceDerivative based on the identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### PUT
##### Summary:

Updates odsInstanceDerivative based on the resource identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### DELETE
##### Summary:

Deletes an existing odsInstanceDerivative using the resource identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Resource was successfully deleted. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/odsInstanceContexts

#### GET
##### Summary:

Retrieves all odsInstanceContexts.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| offset | query | Indicates how many items should be skipped before returning results. | Yes | integer |
| limit | query | Indicates the maximum number of items that should be returned in the results. | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### POST
##### Summary:

Creates odsInstanceContext based on the supplied values.

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Created |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/odsInstanceContexts/{id}

#### GET
##### Summary:

Retrieves a specific odsInstanceContext based on the identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### PUT
##### Summary:

Updates odsInstanceContext based on the resource identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### DELETE
##### Summary:

Deletes an existing odsInstanceContext using the resource identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Resource was successfully deleted. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/claimSets/{id}/export

#### GET
##### Summary:

Retrieves a specific claimSet based on the identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/claimSets

#### GET
##### Summary:

Retrieves all claimSets.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| offset | query | Indicates how many items should be skipped before returning results. | Yes | integer |
| limit | query | Indicates the maximum number of items that should be returned in the results. | Yes | integer |
| sortBy | query |  | No | string |
| descendingSorting | query |  | No | boolean |
| id | query | Claim set id | No | integer |
| name | query | Claim set name | No | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### POST
##### Summary:

Creates claimSet based on the supplied values.

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Created |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/claimSets/{id}

#### GET
##### Summary:

Retrieves a specific claimSet based on the identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### PUT
##### Summary:

Updates claimSet based on the resource identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### DELETE
##### Summary:

Deletes an existing claimSet using the resource identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Resource was successfully deleted. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/authorizationStrategies

#### GET
##### Summary:

Retrieves all authorizationStrategies.

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/applications

#### GET
##### Summary:

Retrieves all applications.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| offset | query | Indicates how many items should be skipped before returning results. | Yes | integer |
| limit | query | Indicates the maximum number of items that should be returned in the results. | Yes | integer |
| sortBy | query |  | No | string |
| descendingSorting | query |  | No | boolean |
| id | query | Application id | No | integer |
| applicationName | query | Application name | No | string |
| claimsetName | query | Claim set name | No | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### POST
##### Summary:

Creates application based on the supplied values.

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Created |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/applications/{id}

#### GET
##### Summary:

Retrieves a specific application based on the identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### PUT
##### Summary:

Updates application based on the resource identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### DELETE
##### Summary:

Deletes an existing application using the resource identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Resource was successfully deleted. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/odsInstances/{id}/applications

#### GET
##### Summary:

Retrieves applications assigned to a specific ODS instance based on the resource identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/vendors/{id}/applications

#### GET
##### Summary:

Retrieves applications assigned to a specific vendor based on the resource identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/actions

#### GET
##### Summary:

Retrieves all actions.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| offset | query | Indicates how many items should be skipped before returning results. | Yes | integer |
| limit | query | Indicates the maximum number of items that should be returned in the results. | Yes | integer |
| sortBy | query |  | No | string |
| descendingSorting | query |  | No | boolean |
| id | query | Action id | No | integer |
| name | query | Action name | No | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /

#### GET
##### Summary:

Retrieve API informational metadata

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/claimSets/copy

#### POST
##### Summary:

Creates claimSet based on the supplied values.

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Created |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/claimSets/import

#### POST
##### Summary:

Creates claimSet based on the supplied values.

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Created |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/claimSets/{claimSetId}/resourceClaimActions/{resourceClaimId}/overrideAuthorizationStrategy

#### POST
##### Summary:

Creates claimSet based on the supplied values.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| claimSetId | path |  | Yes | integer |
| resourceClaimId | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/claimSets/{claimSetId}/resourceClaimActions/{resourceClaimId}/resetAuthorizationStrategies

#### POST
##### Summary:

Creates claimSet based on the supplied values.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| claimSetId | path |  | Yes | integer |
| resourceClaimId | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/claimSets/{claimSetId}/resourceClaimActions

#### POST
##### Summary:

Creates claimSet based on the supplied values.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| claimSetId | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Created |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /connect/register

#### POST
##### Summary:

Registers new client

##### Description:

Registers new client

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Application registered successfully. |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /connect/token

#### POST
##### Summary:

Retrieves bearer token

##### Description:


To authenticate Swagger requests, execute using "Authorize" above, not "Try It Out" here.

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Sign-in successful. |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/claimSets/{claimSetId}/resourceClaimActions/{resourceClaimId}

#### PUT
##### Summary:

Updates claimSet based on the resource identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| claimSetId | path |  | Yes | integer |
| resourceClaimId | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

#### DELETE
##### Summary:

Deletes an existing claimSet using the resource identifier.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| claimSetId | path |  | Yes | integer |
| resourceClaimId | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |

### /v2/applications/{id}/reset-credential

#### PUT
##### Summary:

Reset application credentials. Returns new key and secret.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request. The request was invalid and cannot be completed. See the response body for details. |
| 401 | Unauthorized. The request requires authentication |
| 403 | Forbidden. The request is authenticated, but not authorized to access this resource |
| 404 | Not found. A resource with given identifier could not be found. |
| 500 | Internal server error. An unhandled error occurred on the server. See the response body for details. |
