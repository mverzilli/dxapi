---
category: Devices
path: '/devices/authehtication_token/events/[test_result_guid]/pii'
title: 'Submit PII'
type: 'PUT'

layout: nil
---

Allows submission of Personal Identifiable Information into a previously submitted test result.

# Request

* The path must include a **valid authentication token**.
* The path must include a valid **test result GUID**.
* **The body can't be empty** and must include the PII.

`Authentication: bearer f862f658-ad89-4fcb-995b-7a4c50554ff6`

```/devices/c4c52784-bfd5-717d-7a91-614acd972d5d/events/c4c52784-bfd5-717d-7a91-614acd972d5e/pii```

```{
  "patient_id" : 2,
  "patient_name" : "Lorem Ipsum",
  "patient_telephone_number" : "12345678",
  "patient_zip_code" : "1234"
}```

# Response

**If succeeds**, returns the created [event](#/event-resource).

`Status: 200 Ok`

For errors responses, see the [response status codes documentation](#http-response-codes).