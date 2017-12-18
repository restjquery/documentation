# Comments #

The comments API allows you to create, view, update, and delete individual, or a batch, of comments.

## Comment attributes ##

Attribute | Type | Description
--------- | ------- | -----------
`id` | integer | Unique identifier for the object.
`context` | string | Scope under which the request is made; determines fields present in response.
`force` | boolean | Whether to bypass trash and force deletion.
`password` | string | The password for the parent post of the comment (if the post is password protected).
`author` | integer | The ID for the author of the object.
`author_email` | string | Email address for the object author.
`author_ip` | string | IP address for the object author.
`author_name` | string | Display name for the object author.
`author_url` | string | URL for the object author.
`author_user_agent` | string | User agent for the object author.
`content` | string | The content for the object.
`date` | string | The date the object was published, in the site's timezone.
`date_gmt` | string or datetime | The date the object was published, as GMT.
`parent` | integer | The ID for the parent of the object.
`post` | integer | The ID of the associated post object.
`status` | string | State of the object.
`meta` | object | Meta fields.
