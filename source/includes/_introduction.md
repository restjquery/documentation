# Introduction #

WordPress REST API jQuery is still fresh so there will be changes to the documentation over time as the script is developed.

## Requirements ##

You must be using:

* WordPress 4.4+.
* [WordPress REST API jQuery](https://github.com/seb86/WordPress-REST-API-jQuery) for Web Apps outside of WordPress or use the [WordPress REST API jQuery Support](https://wordpress.org/plugins/wp-rest-api-jquery-support/) plugin for a quick install.
* You may make requests over either HTTP or HTTPS, but HTTPS is recommended where possible.

<aside class="notice">
Please note that you are <strong>not</strong> required to install the <a href="https://wordpress.org/plugins/rest-api/">WP REST API (WP API)</a> plugin.
</aside>

## Parameters ##

Parameter | Default | Description
--------- | ------- | -----------
site_url |  | Default is the current host name. Only set if connecting with another site.
namespace | wp/v2 | Default is current WordPress REST API. Set this to use other REST API's registered like JetPack, WooCommerce etc.
endpoint | `NULL` | [See the endpoints](https://developer.wordpress.org/rest-api/reference/#rest-api-developer-endpoint-reference) for reference.
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

<aside class="notice">Further documentation for using with WooCommerce is currently in the works. Suggest using <a href="http://woocommerce.github.io/woocommerce-rest-api-docs/" target="_blank">WooCommerce REST API Docs</a> for reference purposes only.</aside>

## Tools ##

Some useful tools you can use to access the API include:

* [Postman](https://www.getpostman.com/) - A multi platform REST API GUI client (using Google Chrome or installing the app on Mac OS X or Windows).
* [CocoaRestClient](http://mmattozzi.github.io/cocoa-rest-client/) - A Mac OS X GUI client for interacting with the API.
* [Paw HTTP Client](https://itunes.apple.com/us/app/paw-http-client/id584653203?mt=12) - Another HTTP client for Mac OS X.
* [RESTClient, a debugger for RESTful web services](https://addons.mozilla.org/en-US/firefox/addon/restclient/) - Free Firefox add-on.
* [Advanced REST client](https://chrome.google.com/webstore/detail/advanced-rest-client/hgmloofddffdnphfgcellkdfbfbjeloo) - Free Google Chrome extension.
* [RequestBin](https://requestb.in/) - Allows you test web hooks.
* [Hookbin](https://hookbin.com/) - Another tool to test web hooks.
