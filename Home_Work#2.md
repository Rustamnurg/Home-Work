	//////////////////
	2)
	double a, b, c, d, x1, x2;
	a = Double.valueOf(args[0]);
	b = Double.valueOf(args[1]);
	c = Double.valueOf(args[2]);
	d = 0;
	x1 = 0;
	x2 = 0;

	d = (b * b - 4 * a * c);
	if (d > 0) {
		x1 = (-b + Math.sqrt(d)) / (2.0*a); 
		x2 = (-b - Math.sqrt(d)) / (2.0*a);
		System.out.println("x1 = " + x1 + "; x2 = " + x2);
	} 
	else if (d == 0){
		x1 = (-b) / (2.0*a);
		System.out.println("x = " + x1);	
	} 
	else {
		System.out.println("x = none");	
	}
	
	
	//////////////////
	3)
		for(int i = 1; i < 10; i++) {
		for(int j = 1; j < 10; j++) {
			System.out.print(j + "x" + i + "=" + i * j + "    "); 
		}
		}
		
	//////////////////
	4)A
	double x, y, result, check;
	x = Double.valueOf(args[0]);
	y = Double.valueOf(args[1]);
	result = 0;

	check = 4 / 3 + 5 * x / 2 - 74;
	if(check != 0){
		result = (Math.pow(x, 6) + Math.pow(y, 7) - 37) / check + y * y / 2 - x * y;
		System.out.print(result);
	}
	else {
		System.out.print("Sorry, you can not divide by zero");
	}
	
	
	//////////////////
	4)B
	double x, y, result, check;

	x = Double.valueOf(args[0]);
	y = Double.valueOf(args[1]);
	result = 0;

	check = x * y - Math.pow(y, 3) +3;
	if(check != 0){
		result = (Math.pow(y, 6) + Math.pow(x, 7) - 64) / check - 72 * x + 1 / 8;
		System.out.print(result);
	}
	else {
		System.out.print("Sorry, you can not divide by zero");
	}
	
	//////////////////
	5)
	double s, n, x;

	n = Double.valueOf(args[0]);
	s = x = 1;        

	for (int i = 0; i < n; i++){
	x += 2;
	if(i % 2 == 0){
		s -= 1 / (x * x);
	}
	else {
		s += 1 / (x * x);
	}
	System.out.print(s);


//////////////////
6)
double result, x, n, cosx;
x = Double.valueOf(args[0]);
n = Double.valueOf(args[1]);
result = 1;
cosx = Math.toRadians(x);	
cosx = Math.cos(cosx);
	
	for (int i = 0; i < n; i++){
 	result *= (x + cosx);
	}
 	result *= cosx;
 	System.out.println(result);
