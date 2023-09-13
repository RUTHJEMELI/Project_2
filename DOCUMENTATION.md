# API Documentation  

## Introduction

Welcome to the official documentation for my API. This guide provides comprehensive information on API endpoints, request and response formats, sample usage scenarios and  known limitations.

## Standard Request and Response Formats

# ☸️ Requests

## Create a New Person

- **Endpoint:** `POST /api/`
- **Request Body (JSON):**
  
  {
    "name": "metrine",
  }
  

## Get a Person by ID

**Endpoint:** `GET /api/:user_id`

### Update a Person's Profile

**Endpoint:** `PUT /api/:user_id`

**Request Body (JSON):**


  {
    "name": "Updated Name",

  }

## Delete a Person by ID

**Endpoint:** `DELETE /api/:user_id`

# ☯️ Responses

#### Success Response (HTTP Status 200)

**Response Body (JSON) for GET requests:**

{
  "_id": "12345",
  "name": "metrine",
  
}


#### Error Response (HTTP Status 400)

**Response Body (JSON):**

{
  "error": "internal server error"
}


#  Sample Usage
## Create a New Person
**Request:**


POST /api/
Content-Type: application/json

{
  "name": "metrine",
  
}

### Response (HTTP Status 200):

{
  "_id": "12345",
  "name": "metrine",
  
}


## Get a Person by ID
### Response (HTTP Status 200):

{
  "_id": "12345",
  "name": "metrine",
}


## Update a Person's Profile
## Request:

PUT /api/12345
Content-Type: application/json

{
  "name": "Updated Name",
}
```
# Response (HTTP Status 200):
{
  "_id": "12345",
  "name": "Updated Name",
}

## Delete a Person by ID
## Request:
DELETE /api/12345

## Response (HTTP Status 200):

{
  "_id": "12345",
  "name": "Updated Name",
  
}


