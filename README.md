# testactions2

Simple change in readme.md to test pull request trigger

# to run a repositorydispatch run a post (https://reqbin.com/post-online)
# url
https://api.github.com/repos/githubuser/reponame/dispatches
# Header
Accept: application/vnd.github.v3+json
# Add basic authenticacion with your github token
Permision to repo, admin hook, and delete repo or so
# Content
{ "event_type": "build",
   "client_payload": {
     "env": "development" 
   }
}

# you can retrieve information inside the workflow by
run : echo $ {{ github.event.client_payload.name_of_item_toretrieve }}
