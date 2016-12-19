# voxoco.github.io
VOXO.CO - Our 100% full website migrated from Wordpress to Jekyll and hosted on Netlify! https://www.voxo.co

#### HOW IT WAS DONE

1. Used the `wpstatic` handy tool [here](https://github.com/chnm/WP-Static/blob/master/wpstatic) to export the wordpress site to static html files. This grabs all of the assets, blog posts, etc.. and places the pages in their own directory.
2. Created the jekyll templates in `_layouts` for various page types.
3. Used font matter to inject the layouts for each page.
4. Added repeating content (sidebar and other elements) to `_includes`.
5. Re-factored blog pages and templates to use font matter and migrated blog posts to Markdown.
6. Optimized assets for non blocking js/css loading.

Profit!

#### INSTALL
1. `gem install jekyll`
2. `gem install bundler`
3. `bundle exec jekyll serve`
4. http://localhost:4000

#### ENHANCEMENTS & PLUGINS

Using jekyll seo for social media sharing and general SEO.

Uing somewhat non-conventional way of creating pages. Decided it was easier to sperate pages by adding folders instead of using jekyll permalinks

Put css in `_includes` so they can be injected in the html files (to eliminate additional http calls)

Optimized images using [ImageOptim](https://imageoptim.com/mac)

Google PageSpeed score of 89% for desktop and mobile
