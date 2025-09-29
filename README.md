# Hornazos por el mundo
***Hornazos por el mundo*** (Hornazo is a typical spanish patty, so the name is ***Patties by the world***) We want to create a small blog with recipes and typical dishes of our trips.
For it, we are going to use Jekyll and we will explain how to set up a blog with jenkyll in this *README*.

## Ruby installation with rbenv
To avoid compatibility issues, it is recommended to use rbenv to manage your Ruby version.

1. Install rbenv (on macOS):
   ```sh
   brew install rbenv
   rbenv init
   ```
   Add the following to your ~/.zshrc or ~/.bashrc file:
   ```sh
   export PATH="$HOME/.rbenv/bin:$PATH"
   eval "$(rbenv init -)"
   ```
   Restart your terminal.

2. Install the recommended Ruby version:
   ```sh
   rbenv install 3.2.2
   rbenv global 3.2.2
   ruby -v
   ```

## Installing dependencies with Bundler
1. Install Bundler if you don't have it:
   ```sh
   gem install bundler
   ```
2. Install project dependencies:
   ```sh
   bundle install
   ```

## Configuration
The Jekyll configuration is described in _config.yml file.
- ### You can use two types of configuration:
        bundle exec jekyll serve --config _developer_config.yml
  (one for production (**_config.yml**) and another for development (**_config_dev.yml**))

> **Note:** The command above will only work if the file `_developer_config.yml` (or `_config_dev.yml`) exists in your project directory and contains valid Jekyll configuration. You can create a development config file by copying `_config.yml` and modifying the necessary settings for your local environment.

## Information
- https://jekyllrb.com/
- https://github.com/rbenv/rbenv