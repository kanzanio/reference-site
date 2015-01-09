# Kanzan reference site

A simple reference site for a Kanzan site. This includes examples of each content type that you can manage in a site with Kanzan via http://kanzan.io


## Declaring Kanzan content

Kanzan understands HTML5 data attributes and will look for attributes that start with `data-kanzan-`. All attributes are optional except for `data-kanzan-id` and `data-kanzan-type`.

All kanzan data attributes are removed from the markup when output from Kanzan.io and managed content is subsituted.


## Kanzan attributes

- `data-kanzan-id` - A unique identifier for this field in the file.
- `data-kanzan-type` - The content type for this field.
- `data-kanzan-help` - Optional descriptive help text to display in the content admin site.
- `data-kanzan-label` - Optional label to display in the content admin site (`data-kanzan-id` used if not defined)


## Content types

### text

Defined by `data-kanzan-type="text"`

A simple short plain text field. This will create a text input field in the the content admin site.

```
<h1 data-kanzan-type="text" data-kanzan-id="site-title">The Site Title</h1>
```


### blob

Defined by `data-kanzan-type="blob"`

A longer plain text field. This will create a text area input field in the the content admin site.

```
<div data-kanzan-type="blob" data-kanzan-id="site-intro-text">
	Some longer text which might get very long as your creative juices flow.
</dive>
```


### markdown

Defined by `data-kanzan-type="markdown"`

A longer text field which interprets markdown. This will create a text area input field in the the content admin site.

```
<div data-kanzan-type="markdown" data-kanzan-id="structured-content" data-kanzan-help="Markdown is supported in this section.">
	
	Oooh. Lovely [Markdown](http://daringfireball.net/projects/markdown/syntax)

</div>
```
