

**Example**

```js
var myRestClient; /* create your own RestClient. */


/* basic usage */
myRestClient = new ZigposRtlsRestClient('zigpos-gateway');


/* or if you love working with objects */
myRestClient = new ZigposRtlsRestClient({
	ip : 'zigpos-gateway',
	port : '8083'
	protocol : 'https',
});




/* get all devices from API: */
myRestClient.getAllDevices({
	success : function(data){
		/** [device, device, device, ...] **/
	},
	error : function(error){
		/** handle error **/
	}
});

```



\## License

\[MIT\](http://opensource.org/licenses/MIT)
