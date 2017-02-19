# bulle

## plugin.json
```javascript
{
  //specify path's to saft modules to be loaded
  "modules": ['my-modules/module1.js'],
  // first we look at package.json to resolve plugin dependencies.
  // But if we are dependent on modules purely in runtime/DI we must add them here
  "dependencies": {"@surikat/toolbar": "^1.0.2"},
  // one or more conditions that needs to evaluate to true for this
  // plugin to be included in the build
  // TODO, maybe only support easier profiles=['cordova', 'dev']
  "conditional": ['#/env/cordova==="true"']
}
```