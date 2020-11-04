<p>
  <h2 align="center">Demo for <a href='https://vuejs.github.io/vetur/vti.html'>VTI</a></h2>
</p>

## How this works

A workflow runs `vti diagnostics` on CI and produces these errors:

```
Getting diagnostics from:  [ 'src/App.vue', 'src/components/HelloWorld.vue' ] 

File : /Users/pine/Code/workshop/vti-demo/src/App.vue
Error: Type '{ name: string; }' is missing the following properties from type 'String': charAt, charCodeAt, concat, indexOf, and 41 more.

File : /Users/pine/Code/workshop/vti-demo/src/components/HelloWorld.vue
Error: Property 'name' does not exist on type 'String'.
```

You can run `yarn && yarn type-check` to get these errors on CLI as well.

[This PR](https://github.com/octref/vti-demo/pulls/1) fixes the type error and the build then succeeds.