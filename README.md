

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


/* get positions history for device 873897389716781: */
myRestClient.getPositionHistory({
	address : '873897389716781'
	parameters : [
		'minTimestamp=1589080554345',
		'maxTimestamp=1589080565445',
		'limit=50'
	]
	success : function(data){
		/** [position, position, position, ...] **/
	},
	error : function(error){
		/** handle error **/
	}
});

```
