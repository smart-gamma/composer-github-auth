# composer-github-auth
Ability to store a github auth data at composer.json for multiply deploys 

Follow solution can be applied for the cases when you will need mass github.com calls, like Amazon ASG scalling/deploy

1. curl -u 'githubuser' -d '{"note":"Composer 2"}' https://api.github.com/authorizations
2. put to composer.json

 "config": {
     "bin-dir": "bin",
       "github-oauth": {
          "github.com": "%youroauthtoken%"
        }
   }
