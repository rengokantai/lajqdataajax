# lajqdataajax
##1. Using AJAX and
###4 Fetching JSON data
sunlight foundation api


###7 Solution: ZIP code lookup
ziptastic api.  
A sample
```
$('#zipCode').keyup(function(e){
  var zipCode=$(this).val();
  if(zipCode.length===5&& $.isNumeric(zipCode)){
    var requestURL = 'hhttp://ziptasticapi.com/'+zipCode+'?callback=?';
    $.getJSON(requestURL,null,function(data){
      if(data.city) $('#city').val(data.city);
    })
  }
})
```
