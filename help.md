### Bundle

bundle -v
gem -v
gem list bundler

echo 'export PATH="/c/Ruby34-x64/bin:$PATH"' >> ~/.bashrc

bundle install
bundle exec jekyll serve

### Git

git pull origin main
git commit -am "backup before update"
git push origin main

git remote add upstream https://github.com/cotes2020/chirpy-starter.git
git remote add upstream https://github.com/cotes2020/jekyll-theme-chirpy.git
git fetch upstream
git merge upstream/main

git commit -m "homepage update"
git commit -m "navigation added"

