# Pages #

## Get Pages ##

```javascript
var pages = restjQuery(
  endpoint: "pages"
);
```

> JSON response example:

```json
code response goes here
```

This lets you retrieve pages.

### HTTP Request ###

<div class="api-endpoint">
  <div class="endpoint-data">
    <i class="label label-get">GET</i>
    <h6>/wp-json/wp/v2/pages</h6>
  </div>
</div>

## Get a Single Page ##

```javascript
var sample_page = restjQuery(
  endpoint: "pages/2"
);
```

> JSON response example:

```json
code response goes here
```

This lets you retrieve and view a specific page.

### HTTP Request ###

<div class="api-endpoint">
  <div class="endpoint-data">
    <i class="label label-get">GET</i>
    <h6>/wp-json/wp/v2/pages/2</h6>
  </div>
</div>
