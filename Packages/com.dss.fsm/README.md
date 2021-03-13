# unity-fsm

This is just a fork of thefuntastic's [Unity3d-Finite-State-Machine](https://github.com/thefuntastic/Unity3d-Finite-State-Machine).

I updated it to support recent Unity versions by removing the outdaded unit test framework, and by hosting it on NPM.

Please see the [readme](README-original.md) in the package directory for information on how to use it.

## How To Install

The fsm package uses the [scoped registry](https://docs.unity3d.com/Manual/upm-scoped.html) feature to import
dependent packages. Please add the following sections to the package manifest
file (`Packages/manifest.json`).

To the `scopedRegistries` section:

```
{
  "name": "DSS",
  "url": "https://registry.npmjs.com",
  "scopes": [ "com.dss" ]
}
```

To the `dependencies` section:

```
"com.dss.fsm": "1.0.0"
```

After changes, the manifest file should look like below:

```
{
  "scopedRegistries": [
    {
      "name": "DSS",
      "url": "https://registry.npmjs.com",
      "scopes": [ "com.dss" ]
    }
  ],
  "dependencies": {
    "com.dss.fsm": "1.0.0",
    ...
```