# HexoBookTemplate
This is my hexo book template. I'm going to write book and notes with it.

This template is based on the theme [hexo-theme-book](https://github.com/kaiiiz/hexo-theme-book) and modified on [hexo-theme-book-demo](https://github.com/kaiiiz/hexo-theme-book-demo).



# Usage

1. Clone this repo to local
2. Run `npm install hexo`
3. Run `npm install hexo-renderer-scss --save`
4. Run `npm uninstall hexo-renderer-marked --save`
5. Run `npm install hexo-renderer-markdown-it --save`
6. Run `npm install @iktakahiro/markdown-it-katex`

## Detail Tag

Run `npm install hexo-tag-details --save` to use detail tag.

Use like

```
{% details [mode:open/close] summary text %}
detail text
{% enddetails %}
```

Example1:

```
{% details Where are you from? %}
I'm from the Earth. Water Planet!
{% enddetails %}
```

it generates HTML:

```
<details>
  <summary>Where are you from?</summary>
  I'm from the Earth. Water Planet!
</details>
```

Repo link: https://github.com/hinastory/hexo-tag-details

# Admonition Usage

Run `npm install --save hexo-tag-admonition`

One could modify `theme\book\source\ccs\book.scss` to change or add color:

```scss
.admonition {
	padding: 0 15px;
	margin-bottom: 20px;
	border: 1px solid transparent;
	border-radius: 4px;
	text-align: left;
}

.admonition-title {
	font-weight: bold;
	text-align: left;
}

.admonition.blue,
.admonition.info,
.admonition.tips {
	background-color: #67b2e4;
	border-color: #3498db;
}

.admonition.orange,
.admonition.warn,
.admonition.important {
	background-color: #ec9e59;
	border-color: #e67e22;
}

.admonition.red,
.admonition.critical {
	background-color: #ed796d;
	border-color: #e74c3c;
}

.admonition.gray,
.admonition.critical {
	background-color: #dddddd;
	border-color: #999999;
}
```

you can use by

```
{% admonition <Type:red,gray...> <tytle> %}
Hello this is just a test.
This is an another line.
{% endadmonition %}
```

which will turn into something like this:

```
<div class="admonition danger">
  <p class="admonition-title">Don't do this</p>
  <p>Hello this is just a test.</p>
  <p>This is an another line.</p>
</div>
```

