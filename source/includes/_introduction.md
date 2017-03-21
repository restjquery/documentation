# Introduction #

WordPress REST API jQuery is still fresh so there will be changes to the documentation over time as the script is developed.

## Requirements ##

You must be using:

* WordPress 4.4+.
* You may make requests over either HTTP or HTTPS, but HTTPS is recommended where possible.

<aside class="notice">
Please note that you are <strong>not</strong> required to install the <a href="https://wordpress.org/plugins/rest-api/">WP REST API (WP API)</a> plugin.
</aside>

## Parameters ##

Parameter | Default | Description
--------- | ------- | -----------
site_url |  | Default is the current host name. Only set if connecting with another site.
namespace | wp/v2 | Default is current WordPress REST API. Set this to use other REST API's registered like JetPack, WooCommerce etc.
endpoint | posts | [See the endpoints](https://developer.wordpress.org/rest-api/reference/#rest-api-developer-endpoint-reference) for reference.
post_data | {} | Use this to pass data for posting or updating a request.
form_method | GET | `GET, POST, UPDATE, DELETE`
data_type | json | Use `jsonp` for cross-domain support

<aside class="notice">Endpoint accepts all the standard filter parameters which can be passed as a HTTP query string parameter, e.g. <code>/posts?per_page=5.</code></aside>

## Setting the Site URL ##

```javascript
var posts = restjQuery(
  site_url: "http://example.com"
);
```

This lets you get posts or any other endpoint you set from a specific WordPress site.

## Setting the Namespace ##

```javascript
var products = restjQuery(
  namespace: "wc/v1",
  endpoint: "products"
);
```

This lets you get data from other registered REST API's like WooCommerce as shown in the example. This will also need to be accompanied by the `endpoint` parameter.
