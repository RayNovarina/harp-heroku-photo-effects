cd /Users/raynovarina/Sites/AtomProjects/harp/photo-effects

Created and initialized harp app:

$ /Users/raynovarina/Sites/AtomProjects

$ harp init photo-effects

$ cd photo-effects

Change main.less to:
/* empty */

Change index.jade:
  h1 Welcome to harp/photo-effects.
  h3 Deployed locally at http://localhost:9000/
  h3 Deployed on Heroku at https://harp-photo-effects-94037.herokuapp.com/

Add package.json and Procfile files for Heroku deploy:
  package.json:

    {
      "name": "harp-heroku-photo-effects",
      "version": "1.0.0",
      "description": "A Harp App on Heroku",
      "dependencies": {
        "harp": "*"
      }
    }

  Procfile:

    web: harp server --port $PORT

At github account, create new repository: harp-heroku-photo-effects and then
locally.
  $ git init
  $ git remote add origin https://github.com/RayNovarina/harp-heroku-photo-effects.git

Create Heroku app:
  $ heroku create harp-photo-effects-94037

$ git remote -v
  heroku  https://git.heroku.com/harp-photo-effects-94037.git (fetch)
  heroku  https://git.heroku.com/harp-photo-effects-94037.git (push)
  origin  https://github.com/RayNovarina/harp-heroku-photo-effects.git (fetch)
  origin  https://github.com/RayNovarina/harp-heroku-photo-effects.git (push)

Deploy changes to github and heroku:
  $ git add .
  $ git commit -am "First Harp + Heroku commit"
  $ git push origin master
  $ git push heroku master

View on Heroku:

  https://harp-photo-effects-94037.herokuapp.com shows:

  Welcome to harp/photo-effects.
  Deployed locally at http://localhost:9000/
  Deployed on Heroku at https://harp-photo-effects-94037.herokuapp.com/

------------------------------
Replace with github exploding exploding profiles code and redeploy working
version to Heroku.

Erase all harp files expect for package.json, Procfile.
Clone from github exploding-effects repository into projects/exploding-effects
folder and move those folder into harp/photo-effects.

Because we have no layout.jade file, hard seems to set the app root at
harp/photo-effects.

Load app as is from localhost:9000/pages/management.html

Fixup a lot of problems.
harp less preprocessor seems to only be able to find management.less file if
it is at app root (harp/photo-effects). Gets converted to a .css file when
loaded.

commit and push fixed version to github.
push to heroku.

load heroku version via https://harp-photo-effects-94037.herokuapp.com/pages/management.html

===============================
based on:
https://codepen.io/anon/pen/rwWGME
http://www.hongkiat.com/blog/less-basic/
http://getbootstrap.com/getting-started/#template

http://www.picturetopeople.org/image_effects/photo-halftone/halftone-image-generator.html

https://www.climate.com/about/leadership

=========================================
