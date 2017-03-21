# Post Types #

## Get Post Types ##

```javascript
var post_types = restjQuery(
  endpoint: "types"
);
```

> JSON response example:

```json
code response goes here
```

This lets you retrieve post types.

### HTTP Request ###

<div class="api-endpoint">
  <div class="endpoint-data">
    <i class="label label-get">GET</i>
    <h6>/wp-json/wp/v2/types</h6>
  </div>
</div>

## Get a Single Post Type ##

```javascript
var post_types = restjQuery(
  endpoint: "types/1"
);
```

> JSON response example:

```json
code response goes here
```

This lets you retrieve and view a specific post type.

### HTTP Request ###

<div class="api-endpoint">
  <div class="endpoint-data">
    <i class="label label-get">GET</i>
    <h6>/wp-json/wp/v2/types/1</h6>
  </div>
</div>
