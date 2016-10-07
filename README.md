# SharedStateBehavior

Shared State Behavior for Polymer Elements

Polymer's computed paradigm is strictly hierarchial and often inconvenient for particular types of applications, especially when the
requirement is as simple as for elements to have access to a common shared-property throughout the app. This behavior adds the ability
for elements to share a property without needing to know about each other pass that property hierarchially. Primitive types, Arrays and Objects are supported.

An object using SharedStateBehavior should declare the `SharedStateBehavior` as well as `sharedValue: true` in the definition of the property it wishes to share with other objects which make matching declarations. 

```es6
    {
      behaviors: [
        SharedStateBehavior
      ],
      properties: {
        prop1: {
          type: String,
          value: '',
          sharedValue: true,
        }
    }
```

## Run Demo

```
$ polymer serve
```

## Running Tests

```
$ polymer test
```
