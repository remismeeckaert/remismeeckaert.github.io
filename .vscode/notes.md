docker run --rm -it \
  --volume="$PWD:/srv/jekyll" \
  --volume="$PWD/vendor/bundle:/usr/local/bundle" \
  -p 4000:4000  jekyll/jekyll:latest \
  --name website 
  bundle exec jekyll serve