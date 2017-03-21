# Post Statuses #

## Get Post Statuses ##

```javascript
var post_statuses = restjQuery(
  endpoint: "statuses"
);
```

> JSON response example:

```json
code response goes here
```

This lets you retrieve post statuses.

### HTTP Request ###

<div class="api-endpoint">
  <div class="endpoint-data">
    <i class="label label-get">GET</i>
    <h6>/wp-json/wp/v2/statuses</h6>
  </div>
</div>

## Get a Single Post Status ##

```javascript
var post_statuses = restjQuery(
  endpoint: "statuses/1"
);
```

> JSON response example:

```json
code response goes here
```

This lets you retrieve and view a specific post status.

### HTTP Request ###

<div class="api-endpoint">
  <div class="endpoint-data">
    <i class="label label-get">GET</i>
    <h6>/wp-json/wp/v2/statuses/1</h6>
  </div>
</div>
