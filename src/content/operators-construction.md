# Operators construction

## create

When you are starting out or you just want to test something you tend to start out with the `create()` operator. This takes a function with an `observer` as a parameter. This has been mentioned in previous sections such as [Observable Wrapping](observable-wrapping.md). The siignature looks like the following

```javascript
Rx.Observable.create([fn])
```

And an example looks like:

```javascript
Rx.Observable.create(observer => {
    observer.next( 1 );
})
```

## range

Signature

```javascript
Rx.Observable.range([start],[count])
```

Example

```javascript
let stream$ = Rx.Observable.range(1,3)

// emits 1,2,3
```
