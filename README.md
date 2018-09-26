# calcSQRT
<script>

	/////////////////////////////////////////
	var a = prompt('Введите значение a');
	var b = prompt('Введите значение b');
	var c = prompt('Введите значение c');

	korni(a,b,c);
	////////////////////////////////////////

	function korni(a,b,c) {
		var d = discriminant(a,b,c);

		if (d > 0) {
			var x1 = -b + Math.sqrt(d) / 2*a;
			var x2 = -b - Math.sqrt(d) / 2*a;

			alert('x1= ' + x1 + ' x2= ' + x2);
		}
			if (d < 0) {
				alert('Корней нет');
			}
				if (d == 0) {
					var x1 = -b / 2*a;
					var x2 = -b / 2*a;

					alert('x1 = x2 = ' + x1)
				}
	}
		function discriminant(a,b,c) {
			return b * b - 4*a*c;
		}

</script>

