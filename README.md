pubic class cbv{
  pubic static void main(String[] args){
    int a=10, b=15;
    System.out.println(" 傳值呼叫前\t a="+a+"\t b="+b);
    byVal(a, b);
    System.out.println(" 傳值呼叫後\t a="+a+"\t b="+b);
  }
  static void byVal(int x, int y){
    int t;
    t = x;
    x = y;
    y = t;
    System.out.println(" 傳值呼叫中\t a="+x+"\t b="+y);
  }
}
    
class Obj{
  int a, b;
  Obj(){
    a=10;
    b=15;
  }
}
pubic class cbr{
  pubic static void main(String[] args){
    Obj obj = new Obj;
    System.out.println((" 參考呼叫前\t a="+a+"\t b="+b);
    byRef(obj)
    System.out.println((" 參考呼叫前\t a="+a+"\t b="+b);
  }

  static void byRef(int p){
    int t;
    t = p.a;
    p.a = p.b;
    p.b = t;
  }
}

    
    
public class fib {
    
    public static void main(String args[])throws IOException {
     	Scanner s = new Scanner(System.in);
     	System.out.print("計算費氏數列的第X項，請輸入X=");
     	int x =s.nextInt();
     	System.out.println("費氏數列第"+x+"項="+fib(x));
    }
    
    public static long fib(int n){
        if(n==1)
		return 1;
	else if (n==2)
		return 1;
	else
		return fib(n-1)+fib(n-2); 
    }   
}


public class Fib{

 public static void main(String[] args) {
    
    Scanner s = new Scanner(System.in);
    System.out.print("計算費氏數列的第X項，請輸入X=");
    int x =s.nextInt();
    System.out.println("費氏數列第"+x+"項="+fib(x));
}
  

 public static long fib(int x){

  if(x==1||x==2){

   return 1;

  }else {

   return fib(x-1)+fib(x-2);

  }  

 }  

}
