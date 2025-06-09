# Cognibotics Lab's website

- Version: Jekyll 4.4.1

# Development
- Create jekyll and gems
``` shell
gem install jekyll bundler
```

- Create new website
``` shell
jekyll new website_name --blank
```

- Or pull from github
``` shell
git clone https://github.com/tuantdang/cogniboticslab.git
```

# Build
``` shell
bundle exec jekyll serve
```

# Design
- Please make changes as your own design at **_layout/default.html**
- Specific page located at **_inlcude/*.html** and **markdown files**: *.markdown
- Database: **_data**


# Deployment
Find the result of static web pages (*.html) at **_site** directory.