# Test
public class Calculator {
	public static void main(String[] args) {
		double a ;
		double b ;
		double result ;
		char operator;
		Scanner input = new Scanner(System.in);
		System.out.println("Choose an operator: +,-,*,/");
		operator = input.next().charAt(0);
		System.out.println("Enter first input ");
		a= input.nextDouble();
		System.out.println("Enter Second input");
		b=input.nextDouble();
		switch(operator) {
		case '+':
			result=a+b;
			System.out.println(a+"+"+b+"="+result);
			break;
		case '-':
			result=a-b;
			System.out.println(a+"-"+b+"="+result);
			break;
		case '*':
			result=a*b;
			System.out.println(a+"*"+b+"="+result);
			break;
		case '/':
			result=a/b;
			System.out.println(a+"/"+b+"="+result);
			break;
			
			default:
				System.out.println("Invalid Operator");
		}
		input.close();
	
	}

}
