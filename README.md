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

$curl 'localhost:3000/api/posts/38?begin=0&length=10'
$curl -H "Content-Type: application/json" -X POST -d '{"text":"hello there","title":"post"}' http://localhost:3003/api/posts


$curl -X PUT -H "Content-Type: application/json" -d @post.json localhost:3000/api/post/38