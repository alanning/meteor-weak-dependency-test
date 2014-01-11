meteor-weak-dependency-test
===========================

A small test of Meteor's weak dependency resolution.

Please test on your machine:

```sh
# If Meteor isn't installed yet...
# $ curl https://install.meteor.com/ | sh

$ git clone https://github.com/alanning/meteor-weak-dependency-test.git
$ cd meteor-weak-dependency-test
$ meteor
```

Does the server console say:
```sh
=> Meteor server running on: http://localhost:3000/
[weak-test] iron-router package found? false
undefined
```

or: 

```sh
=> Errors prevented startup:

While building package `weak-test`:
error: no such package: 'iron-router'

=> Your application has errors. Waiting for file change.
```
