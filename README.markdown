Just a simple HTML5 localStorage wrapper written in Javascript

To use, just simply do the following:

	<script src='/path/to/the/localstorage/js/file/utils.storage.js'></script>
	<script>
  	  var storage = utils.storage;
	  storage.init("mynamespace", true);
	  storage.save("mypersonalvar", {someindex: 'somevalue'});
	  if( storage.exists("mypersonalvar") ) {
	    var result = JSON.parse( storage.read("mypersonalvar") );
	    alert( "someindex: " + result.someindex );
	  }
	</script>
