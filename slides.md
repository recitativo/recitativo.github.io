Slideshow
=========

To display any markdown file in slideshow, access slideshow like follow.

```
https://recitativo.github.io/slideshow.html?md=[URL or path to markdown file]
```

To set relative path for markdown file, set its path from `/slideshow.html`.

Also, you can set window title and theme like follow.

```
https://recitativo.github.io/slideshow.html?md=[URL or path to markdown file]&title=[window title]&theme=[theme name or URL for css]
```

Notes:
* [Slideshow for this page](slideshow.html?md=slides.md&title=Slideshow&theme=sky)
* After opening slideshow, press `s` key to show `Note:` segment in presenter window.

---

Customized settings in this slideshow
-------------------------------------

Scripting to render followings:

----

### Horizontal pagenation

3 hyphens with blank lines before and after.

  ```
  [Previous page]
  
  ---
  
  [Next page]
  ```

----

### Vertical pagenation

4 hyphens with blank lines before and after.

  ```
  [Previous page]
  
  ----
  
  [Next page]
  ```

----

### Presenter notes

Line starts with `Note:` or `Notes:` until pagenation.

  ```
  [Previous page]
  
  Notes:
  something to talk, but not to show.
  
  ---
  
  [Next page]
  ```

---

`reveal.js`
-----------

Slideshow functionality on this site uses [`reveal.js`](https://github.com/hakimel/reveal.js).

This slideshow is realized by [`slideshow.html`](https://github.com/recitativo/recitativo.github.io/tree/master/slideshow.html) customized from sample `index.html` of `reveal.js` in [this site's repository](https://github.com/recitativo/recitativo.github.io).

---

How to apply `slideshow.html` into your site
--------------------------------------------

1. Download [`reveal.js`](https://github.com/hakimel/reveal.js/releases).
2. Extract `reveal.js-x.x.x.zip` and put extracted directory into your site.
3. Download [`slideshow.html`](https://raw.githubusercontent.com/recitativo/recitativo.github.io/master/slideshow.html) and put it on upper of your `reveal.js/` directory, i.e. `../reveal.js/`.
4. Check differences between `index.html` in `reveal.js` directory and `slideshow.html`, fix them if it does not work.

Note:
Press `down` key to go page vertically.

----

How to update `reveal.js` in your site
--------------------------------------

1. Download latest [`reveal.js`](https://github.com/hakimel/reveal.js/releases).
2. Rename old `reveal.js/` directory to `rename.js.old/` or etc.
3. Extract `reveal.js-x.x.x.zip` and put extracted directory as `reveal.js` into your site.
4. Check differences between `reveal.js.old/index.html` and `reveal.js/index.html` and apply changes into your `slideshow.html`.

----

Customization in `slideshow.html` against `index.html` in `reveal.js` was submitted as [Pull Request](https://github.com/hakimel/reveal.js/pull/2575). If this PR merged, we can use the original `index.html` without `slideshow.html`.
