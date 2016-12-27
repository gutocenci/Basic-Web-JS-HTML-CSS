			function somar(){
			var n1 = parseInt(document.getElementById("num1").value);
				var n2 = parseInt(document.getElementById("num2").value);
				var resultado = n1 + n2;
				document.getElementById("result").innerHTML = resultado;
			}
			
			function subtrair(){
				var n1 = parseInt(document.getElementById("num1").value);
				var n2 = parseInt(document.getElementById("num2").value);
				var resultado = n1 - n2;
				document.getElementById("subtrair").value = resultado;			
			}
			
			function multiplicar(){
				var n1 = parseInt(document.getElementById("num1").value);
				var n2 = parseInt(document.getElementById("num2").value);
				var resultado = n1 * n2;
				alert(resultado);
			}
			
			function option(){
				if(document.getElementById("linha1").checked == true) {
				  alert("Retire um certificado !" + "| Nota: " + 10);
					}
					else if(document.getElementById("linha2").checked == true) {
					  alert("Estude mais para prova de certificado" + "| Nota: " + 7);
					}
					else if(document.getElementById("linha3").checked == true) {
						alert("Aprenda mais estruturas e padrões" + "| Nota: " + 5);
					}
					else if(document.getElementById("linha4").checked == true) {
						alert("Já é um começo, mas falta muito estudo mais" + "| Nota: " + 3);
					}
					else if (document.getElementById("linha5").checked == true) {
						alert("Começe a estudar sintaxe, estruturas e padrões do zero" + "| Nota: " + 0);
					}
					else{
					}
			}
			
			function validar(){
			var msgerro ="";
				if (document.form.user.value == ""){
					document.form.user.focus();
					msgerro = msgerro + "\nDigite o do nome usuario"
				}
				if (document.form.pass.value.length < 10){
					msgerro = msgerro + "\nDigite uma senha com no minimo 10 digitos"
					document.form.pass.focus();
				}
        if(document.form.combo.value == 1){
          msgerro = msgerro + "\nSelecione uma dos tipos de matricula"
          document.form.combo.focus();
        }
				if(document.form.check1.value == "" || document.form.check2.value == ""){
					msgerro = msgerro + "\nSelecione ao menos uma sexo"
					document.form.check.focus();
				}
				if(document.form.email.value == "" ||
					document.form.email.value.indexOf('@')==-1 ||
					document.form.email.value.indexOf('.')==-1){
					msgerro = msgerro + "\nEMAIL NAO DEVE SER VAZIO, E CONTER @ E ."
					document.form.email.focus();
				}
        alert(msgerro);
			}