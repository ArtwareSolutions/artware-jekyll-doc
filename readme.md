### [OSX](https://jekyllrb.com/docs/installation/macos/)

xcode-select --install
export SDKROOT=$(xcrun --show-sdk-path)

### [RVM](https://github.com/rvm/rvm#any-other-operating-system) 

\curl -sSL https://get.rvm.io | bash -s stable 
rvm get stable         

### [Ruby](https://github.com/rvm/rvm#installing-ruby)

rvm install 2.7 --default   
rvm use default 
ruby -v
which ruby

### [Jekyll](https://jekyllrb.com/docs/installation/macos/#install-jekyll)

If you're using Zsh, update PATH and start new terminal:

echo 'export PATH="$HOME/.gem/ruby/2.7.0/bin:$PATH"' >> ~/.zshrc

gem install --user-install bundler jekyll

gem install jekyll bundler


### [Create new site](https://jekyllrb.com/docs/#instructions)

jekyll new artware-doc

cd artware-doc

bundle exec jekyll serve

bundle exec jekyll serve --livereload

### [git](https://docs.github.com/en/get-started/importing-your-projects-to-github/importing-source-code-to-github/adding-an-existing-project-to-github-using-the-command-line)

git init -b main

git add . && git commit -m "initial commit"

gh repo create artware/artware-doc

git remote add origin https://github.com/ArtwareSolutions/artware-doc.git

git remote -v

git push -u origin main
