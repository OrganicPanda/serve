# serve

A fork of [TJ](https://github.com/tj)'s [serve](https://github.com/tj/serve).

This version has an extra option that allows json files to be used as rest endpoints. This readme will only document my changes. For a complete readme please refer [upstream](https://github.com/tj/serve).

**This is intended for rapid prototyping purposes only. You would be mad to use this on any real project.**

## Installation
```shell
npm install serve-with-mock-rest
```

## Usage
Firstly create a json file that contains an array at the top level. `[]` is the minimum but you can fill it with existing objects if you wish.

```shell
serve --rest
```

Now you can `GET`, `PUT`, `PATCH`, `POST` and `DELETE` to that file as if it were a rest endpoint. 

For more information see [connect-mock-rest`](https://github.com/OrganicPanda/connect-mock-rest) which is the middleware that provides this functionality.