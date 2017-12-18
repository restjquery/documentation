## List pages ##

This API helps you to list all the pages that have been created.

### HTTP Request ###

<div class="api-endpoint">
  <div class="endpoint-data">
    <i class="label label-get">GET</i>
    <h6>/wp-json/wp/v2/pages</h6>
  </div>
</div>

```javascript
var pages = restjQuery(
  endpoint: "pages"
);
```

> JSON response example:

```json
code response goes here
```

## Retrieve a page ##

This API helps you to retrieve and view a specific page by ID.

```javascript
var sample_page = restjQuery(
  endpoint: "pages/2"
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
    <h6>/wp-json/wp/v2/pages/2</h6>
  </div>
</div>
