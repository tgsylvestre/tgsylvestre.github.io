---
title: "Jekyll Remote Theme Support Added"
image: 
  path: /assets/images/chocolate-chip-cookies-lg.jpg
  thumbnail: /assets/images/chocolate-chip-cookies-400x200.jpg
  caption: "Photo from [Pexels](https://www.pexels.com)"
excerpt:
last_modified_at: 2017-12-01T09:51:16-05:00
tags: 
  - Jekyll
---

Basically Basic can now be installed remotely for use on GitHub Pages!

The days of having to forking this repo and manually manage updates are over. Simply install the [**jekyll-remote-theme**](https://github.com/benbalter/jekyll-remote-theme) plugin by doing the following and away you go.

1. If you've previously forked this repo start by removing `_layouts`, `_includes`, `_sass`, `assets/javascripts`, and `assets/stylesheets`. Be sure to leave any files that you've customized so they override the versions bundled in the theme.

2. In your `Gemfile` replace `gem "jekyll"` with the following:

   ```ruby
   gem "github-pages", group: :jekyll_plugins
   gem "jekyll-remote-theme"
   ```

3. Run `bundle update` and verify that all gems install properly.

4. Add `remote_theme: "mmistakes/jekyll-theme-basically-basic"` to your `_config.yml` file.

5. Then add [`jekyll-remote-theme`](https://github.com/benbalter/jekyll-remote-theme) to the `plugins` (previously gems) array in your `_config.yml` file like so:

   ```yaml
   plugins:
     - jekyll-remote-theme
   ```
