import java.util.*;
public class Test{
    static int evaluatepostfix(String exp)
    {
        Stack<Integer> stk = new Stack<>();
        for(int i=0;i<exp.length();i++)
        {
            char c = exp.charAt(i);
            if(Character.isDigit(c))
            stk.push(c- '0');
            else{
                int val1=stk.pop();
                int val2=stk.pop();
                switch(c){
                    case '+':
                        stk.push(val2 + val1);
                        break;
                    case '-':
                        stk.push(val2 - val1);
                        break;
                    case '/':
                        stk.push(val2 / val1);
                        break;
                    case '*':
                        stk.push(val2 * val1);
                        break;
                }
            }
        }
        return stk.pop();
    }
    public static void main(String args[])
    {
        System.out.println("Enter prefix: ");
        Scanner sc=new Scanner(System.in);
        String exp=sc.nextLine();
        sc.close();
        int result = evaluatepostfix(exp);
        System.out.println("Result: " + result);
        
    }
}
