<! DOCTYPE html>
<html>
<title> UKG</title>
<script>
var page=1;
      function validate(opt,pos){
	document.getElementById("1").disabled=true;
	document.getElementById("2").disabled=true;
	document.getElementById("3").disabled=true;
	
	if(opt=='postoffice'){
		document.getElementById(pos).src="correct.png";
		document.getElementById(pos).disabled=false;
                                       document.getElementById(pos).height="100";
		document.getElementById(pos).width="100";
	}
	else{
		document.getElementById(pos).src="wrong.png";
		document.getElementById(pos).disabled=false;
		document.getElementById(pos).height="100";
		document.getElementById(pos).width="100";
	}
	return false;
      }
   function next(){
	if(page<=3)
		page++;
   }

  function prev(){
	if(page>1)
		page--;
  }	
</script>

<body>
    <h2 style="color:red;" align="center">GGV Digital School</h2><h4 align="center"> Match Community helpers with their Workplace</h4>

   <table align="Center">
	<tr >
		<td rowspan="3" width="400px"><img align="center" height="300px" width="300px" src="postman.png"/></td>
		<td><a href="" onclick="return validate('school',2)"><img height="180px" width="300px" src="school.jpg"/></a></td>
		<td><img id="2" src="" disabled="true"></td>
	</tr>
	<tr>
		<td><a href="" onclick="return validate('postoffice',1)"><img height="180px" width="300px" src="postoffice.jpg"/></a></td>
		<td><img id="1" src="" disabled="true"></td>
	</tr>
	<tr width="300px">
		<td><a href="" onclick="return validate('hospital',3)"><img height="180px" width="300px" src="hospital.jpg"/></a></td>
		<td align="center"><img id="3" src="" disabled="true"></td>
	</tr>
	<tr>
		<td colspan="3"><img onclick=prev() src="prev.png" id="prev" height="60" width="60"> 
		<img onclick=next() align="right" src="next.png" id="prev" height="60" width="60"></td>
	</tr>
</table>
<span align="center">
&#169; Copyright by Iniyan
</span>
</body>

</html>
