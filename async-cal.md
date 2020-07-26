# Asynchronous 

## Promisify
```js
const promisify = (cb) => return new Promise((resolve, reject) => {
    cb((error, result) => {
        if(error){
          reject(error)
        } else {
          resolve(result)
        }
      })
  })
```



## Use then chain to handle promise

```js
doSomething().then((res) => console.log('resolved'), (rej) => console.log('rejected'))

```

## Use async to handle promise
```js
async{
  try{
    await doSomething()
  } catch(error){
    console.error(error)
  }
}()
```
