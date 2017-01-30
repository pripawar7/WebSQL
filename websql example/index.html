<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<title>Survey Form And WebSQl</title>
	<style>
		#showForm{
			color:black;
			font-size:25px;
		}

		#showForm table{
			border-collapse:collapse;
			font-family: "Times New Roman", Helvetica, sans-serif;
			font-size:20px;
		}

		#showTab th, #showTab td,#showForm table{
			border:3px solid black;
			padding:7px;
		}

		#colordiv{
			border:2px solid black;
			width: 500px;
			height:400px;
			padding:12px;
		}

		p{
			text-align: left;
		}

		body{
			font-family: "Times New Roman", Helvetica, sans-serif;
			font-size:15px;
			color:black;
		}

	</style>
</head>
<body onLoad="showData()">
	<center><h1>Survey Form And WebSQl</h1></center>
	<center><form>
		<div id="colordiv">
			<p>Color : &nbsp;&nbsp;&nbsp;&nbsp;<input type="color" id="col"></p>
			<p>Number : <input type="number" id="num"></p><br><br>
			<button onclick="save()">SAVE</button>
		</div>
	</form></center>
	<br><br>
	<div id="showForm"></div>
</body>
<script>
		//Open the Database
		if (window.openDatabase) 
			var db = openDatabase('mydb', '1.0', 'Test DB', 2 * 1024 * 1024);
		else
			alert("The form does not support your Browser !!!");

		//Error Log Message
		function error_log(error){
			console.log(error.message);
		}

		//Create Table
		db.transaction(function (tx){
				tx.executeSql('CREATE TABLE IF NOT EXISTS COLORVAL(id INTEGER PRIMARY KEY AUTOINCREMENT,color text,number text)',[]);
		},error_log);

			//Save the Data
			function save(){
				db.transaction(function(tx){
						var colorVal = document.getElementById('col').value;
						var numberVal = document.getElementById('num').value;
						tx.executeSql('INSERT INTO COLORVAL(color,number) VALUES(?,?)',[colorVal,numberVal]);	
						alert("The Color Value is " + colorVal);
						alert("The number Value is "+ numberVal);
     			},error_log);
		}

		//Display the Data
		function showData(){
			db.transaction(function(tx){
				tx.executeSql('SELECT * FROM COLORVAL',[],function(tx,results){ 
				var len = results.rows.length;
				var table ='<table id="showTab">';
				table+='<tr><th style="width:100px;">COLOR</th><th>NUMBER</th>';
				for(var i=0; i<len; i++){
					var data = results.rows.item(i);
					table+='<tr>';
					table+='<td >'+ data.color + '</td><td>' + data.number+'</td>';
					table+='</tr>';
				}
				table+='</table>';
				document.getElementById('showForm').innerHTML = table;
			});
		});
}
</script>
</html>

