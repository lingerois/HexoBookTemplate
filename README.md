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
7. Run `npm install hexo-tag-details --save` to use detail tag.



## Detail Tag

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

