[![Netlify Status](https://api.netlify.com/api/v1/badges/45e344d0-c7db-43ee-8f16-67ec5302b244/deploy-status)](https://app.netlify.com/sites/pmartin/deploys)

Based on the Jekyll [researcher theme](https://github.com/ankitsultana/researcher) by Ankit Sultana.

### Local preview
```
bundle exec jekyll serve
```


### Customization

* You can edit the `.md` (markdown) files as you see fit. You can also add some other markdown file, say `foo.md` in the root directory of the repository. It will then be accessible like so `{{ url of your website }}/foo`.

* You can of course remove `contact.md` if you don't want it

* To set the heading, edit the `title` variable in `_config.yml`

* To edit the `links` mentioned on the navigation bar, you can edit `_config.yml`. For example:

```
nav:
 - name: "About"
   link: "/researcher/"
 - name: "Resume"
   link: "resume.pdf"
 - name: "Contact"
   link: "contact"
```

* You can change the accent (color of hyperlinks) by editing the `accent` variable in `_sass/vars.scss`

* You can setup google analytics, by setting `tracking_id` in `_config.yml`

* To add a profile picture, make sure to give the image tag the class `profile-picture`. In other words,do it like so:

```html
<img class="profile-picture" src="sherlock.jpg">
```

* You can remove/customize the footer as you like by setting the
appropriate variables in `_config.yml`

* (New in v1.2.0) You can add institute logo at the top, by setting `ins_logo` in `_config.yml`. If you want
to adjust the logo's size, try setting `max-height` in `#ins-logo` in file `./_sass/_style.scss` to the desired
value

**Note:** Customizing the accent color might cause merge conflicts if you later try to merge from `bk2dcradle/researcher` to fetch updates/patches etc. (applicable only if you have forked).

### License

[GNU GPL v3](https://github.com/bk2dcradle/researcher/blob/gh-pages/LICENSE)
