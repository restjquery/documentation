# Authentication #

You can authenticate with the API over HTTPS. The site must support SSL. Remember that the Index endpoint will indicate if the site supports SSL.

There are two methods of authentication. HTTP Basic or Cookie Authentication.

### HTTP Basic Auth ###

You may use [HTTP Basic Auth](http://en.wikipedia.org/wiki/Basic_access_authentication) by providing the WordPress username and password. However this method requires sending your username and password with every request, and should only be used for development and testing i.e. not in a production environment.

> HTTP Basic Auth example updating "Hello World" post title.

```javascript
var data = {
  "title": "Kitty",
};

restjQuery(
  endpoint: "posts/1",
  authorization: {
    authorized_method: "basic",
    username: "test123",
    password: "ABCxyz"
  },
  formMethod: "POST",
  postData: data
);
```

### Cookie Authentication ###

In order to authenticate via Cookie Authentication you must be logged in and get the **_wpnonce** data parameter to authorize requests.

> Cookie Authentication example updating "Hello World" post title.

```javascript

var data = {
  "title": "Kitty",
};

restjQuery(
  endpoint: "posts/1",
  nonce: "139eb45874",
  formMethod: "POST",
  postData: data
);
```
