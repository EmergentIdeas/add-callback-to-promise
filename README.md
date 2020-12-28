# Install

npm i --save add-callback-to-promise

# Use

Makes it easier to create a function which returns a Promise but also allows 
a user to specify a callback.

# Example

```js
function somethingLongrunning(options, callback /*optional*/)
	let p = new Promise((resolve, reject) => {
			// Some code here

			if(err) {
				return reject(err)
			}
			resolve(result)
		})
	})
	return addCallbackToPromise(p, callback)
}
```