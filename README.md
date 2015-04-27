Rest Blog
=========

Project for trainings

To start the app

```
$ npm install -g bower
$ npm install
$ bower install
$ node server/main
```
REST API examples:

```
# get posts from 0 to 10 reverse historical order
$curl 'localhost:3000/api/posts?begin=0&length=10'

# get one post by ID
$curl 'localhost:3000/api/posts/38'

# add a post
$curl -H "Content-Type: application/json" -X POST -d '{"text":"hello there","title":"post"}' http://localhost:3003/api/posts


$curl -X PUT -H "Content-Type: application/json" -d @post.json localhost:3000/api/post/38

# post comment
$curl -X POST -H "Content-Type: application/json" -d '{"text":"I am comment","title":"comment"}' http://localhost:3003/api/posts/1/comments

# update comment
$curl -X PUT -H "Content-Type: application/json" -d '{"text":"I AM GRUTE","title":"comment"}' http://localhost:3003/api/posts/1/comments/3

#delete comment
$curl -X DELETE http://localhost:3003/api/posts/1/comments/3
```