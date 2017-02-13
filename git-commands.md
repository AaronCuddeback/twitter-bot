
These are to push update changes to git/heorku

git init 
heroku git:remote -a aaron-twitterbot
git add .
git commit -m 'add environment variables' 
git push heroku master

if errors:

heroku ps:scale worker=0
heroku ps:scale worker=1

check if its running:

 heroku logs -t