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

    Welcome to Harp test app running locally.

    This is yours to own. Enjoy.
