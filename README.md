<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<title>Untitled Document</title>
</head>

<body>
<form>
<table border="1" cellpadding="0" cellspacing="0" align="center">
<tr>
<td>Name</td>
<td><input type="text" id="textid" name="text1" value="" onblur="getValid()"/></td></tr>
    <span id="text_valid"></span>
<tr>
<td colspan="2" align="center"><input type="submit" name="submit" value="submit" />
</table>
</form>
</body>

</body>
<script>
    function isEmpty(str){
        return !str.replace(/\s+/, '').length;
    }
    function getValid(){
         var text=document.getElementById('textid').value;
         if(isEmpty(text)){
         document.getElementById("text_valid").innerHTML = "Enter Text";
         document.getElementById("text1").focus();
         }
         else{
         document.getElementById("text_valid").innerHTML = "";
         }       
    }
</script>

</html>
