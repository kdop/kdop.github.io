# Install ruby, jekyll, and bundler
follow this -> https://jekyllrb.com/docs/installation/ubuntu/

# Install project dependencies
bundle install

# Install workaround for ruby 3:
bundle add webrick 

# Run locally
bundle exec jekyll build && bundle exec jekyll serve

Now browse to http://localhost:4000

Workflow:

# Deploy on PROD machine:
1. Work with snippets and save them.
2. Do changes in blog (this project) and/or regenerate pages to pull in snippet updates. Make sure that org mantarini is public and repo is public. These can be turned to private later.
3. Save any changes in blog (this project).
4. Restart docker server