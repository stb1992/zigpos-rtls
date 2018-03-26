# zigpos-rtls
zigpos rtls client tools



\## Example

```js
var myRestClient; /* create your own RestClient. */


/* simple usage */
myRestClient = new ZigposRtlsRestClient('zigpos-gateway');


/* adding advanced parameters */
myRestClient = new ZigposRtlsRestClient('zigpos-gateway', '8083', 'https');


/* or if you love working with objects */
myRestClient = new ZigposRtlsRestClient({
	ip : 'zigpos-gateway', /* mendatory */
	port : '8083' /* optional, '8083' by default */
	protocol : 'https', /* optional, 'http' by default */
});

```

\## License

\[MIT\](http://opensource.org/licenses/MIT)
