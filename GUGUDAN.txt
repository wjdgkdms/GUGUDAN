package test_java00;
import java.util.*;
public class Gugudan_v3 {

	public static void main(String[] args) {
		int x,y;
		Random r = new Random();
		
		 if(args.length==0){
	         x = Math.abs(r.nextInt() % 9) + 1;
	      }else {
	         x=Integer.parseInt(args[0]);
	      }
		 
		 
		y=Math.abs(r.nextInt()%9)+1;
		
		int num = x*y;
		
		System.out.println();
		System.out.println("* 구구단 "+x+"단에 대한 문제입니다");
		System.out.println();
		
		System.out.println(x+" * "+y+" = ");
		Scanner sc = new Scanner(System.in);
		int F = sc.nextInt();
		
		if(num==F) {
			System.out.println("맞았습니다!");
		}else {
			System.out.println("틀렸습니다");
		}
		System.out.println("입력된 데이터는 아래와 같습니다");
		System.out.println("-----------------------------");
		
		
		for(int i=0; i<args.length; i++) {
			System.out.println("args["+i+"]"+args[i]);
		}
		
			
	}
}
