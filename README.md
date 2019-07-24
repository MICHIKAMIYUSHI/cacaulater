# cacaulater<!DOCTYPE html>
    <head>
        <meta charset="utf-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
        <title></title>
        <meta name="description" content="">
        <meta name="viewport" content="width=device-width">
		
    </head>
	
	<script src="http://code.jquery.com/jquery-latest.min.js"></script>
	
	<script>
		$(document).ready(function() {
			
			$('#plus').click(function() {
				
				var a = Number($('#num1_input').val());
				var b = Number($('#num2_input').val());
			
				$('#result').text(a+b);
								
			})
		})
		$(document).ready(function() {
			
			$('#minus').click(function() {
				
				var a = Number($('#num1_input').val());
				var b = Number($('#num2_input').val());
			
				$('#result').text(a-b);
								
			})
		})
		$(document).ready(function() {
			
			$('#dul').click(function() {
				
				var a = Number($('#num1_input').val());
				var b = Number($('#num2_input').val());
			
				$('#result').text(a*b);
								
			})
		})
		$(document).ready(function() {
			
			$('#divide').click(function() {
			
				var a = Number($('#num1_input').val());
				var b = Number($('#num2_input').val());
				
				if(b<=0){
					alert("안됩니다.");
				}else{
					
					$('#result').text(a/b);
				}
			})
		})
		
	</script>
	
	<body>
		<input id="num1_input" type="number" ></input>
		
		<input id="num2_input" type="number" ></input>
		
		<div id="result" ></div>
		<div>
			<button id="plus">더하기</button>
		
			<button id="minus">뺴기</button>
		
			<button id="dul">곱하기</button>
		
			<button id="divide">나누기</button>
		</div>
    </body>
</html>
