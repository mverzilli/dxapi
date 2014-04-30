---
category: Applications
path: '/api/events'
title: 'Retrieve specific event'
type: 'GET'

layout: nil
---

This method allows applications to retrieve the private patient information for a given test result.

# Request Parameters

```/events/test_result_id```

* The path must include a **valid test_result_id**.
* ```test_result_id``` - id of the desired test result.

### Example

```/events/2```

# Response

```Status: 200 OK```

Returns an [event](#/event-resource)

For errors responses, see the [response status codes documentation](#http-response-codes).