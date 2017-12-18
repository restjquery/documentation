## Retrieve comments ##

This API helps you to list all the comments that have been created.

```javascript
var comments = restjQuery(
  endpoint: "comments"
);
```

> JSON response example:

```json
code response goes here
```

### HTTP Request ###

<div class="api-endpoint">
  <div class="endpoint-data">
    <i class="label label-get">GET</i>
    <h6>/wp-json/wp/v2/comments</h6>
  </div>
</div>

## Retrieve a comment ##

This API helps you to retrieve and view a specific comment by ID.

```javascript
var comments = restjQuery(
  endpoint: "comments/1"
);
```

> JSON response example:

```json
code response goes here
```

### HTTP Request ###

<div class="api-endpoint">
  <div class="endpoint-data">
    <i class="label label-get">GET</i>
    <h6>/wp-json/wp/v2/comments/1</h6>
  </div>
</div>
