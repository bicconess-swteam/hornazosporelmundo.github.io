# Hornazos por el mundo
***Hornazos por el mundo*** (Hornazo is a typical spanish patty, so the name is ***Patties by the world***) We want to create a small blog with recipes and typical dishes of our trips.
For it, we are going to use Jekyll and we will explain how to set up a blog with jenkyll in this *README*.

## First Steps:
- ### Install jekyll
        gem install bundler jekyll
- ### Generate jekyll files
        jekyll new . --force
- ### To test your changes on your computer
        bundle exec jekyll serve

## Configuration
The Jekyll configuration is described in _config.yml file.
- ### We could have two types of configuration:
        bundle exec jekyll serve --config _developer_config.yml
  (one for production (**_config.yml**) and other for develop (**_config_dev.yml**))


More information -> https://jekyllrb.com/