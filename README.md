git checkout --orphan gh-pages
git rm -rf .
cp -r ../dist/* .
git add .
git commit -m "Deploy to gh-pages"
git push -u origin gh-pages --force