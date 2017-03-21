# Comments #

## Get Comments ##

```javascript
var comments = restjQuery(
  endpoint: "comments"
);
```

> JSON response example:

```json
code response goes here
```

This lets you retrieve comments.

### HTTP Request ###

<div class="api-endpoint">
  <div class="endpoint-data">
    <i class="label label-get">GET</i>
    <h6>/wp-json/wp/v2/comments</h6>
  </div>
</div>

## Get a Single Comment ##

```javascript
var comments = restjQuery(
  endpoint: "comments/1"
);
```

> JSON response example:

```json
code response goes here
```

This lets you retrieve and view a specific comment.

### HTTP Request ###

<div class="api-endpoint">
  <div class="endpoint-data">
    <i class="label label-get">GET</i>
    <h6>/wp-json/wp/v2/comments/1</h6>
  </div>
</div>
