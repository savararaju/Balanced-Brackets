# Balanced-Brackets



 public class aditya {
 static boolean   isValid(String s) {
    Stack<Character>st=new Stack();
        for(int i=0;i< s.lenght(); i++)
        {
            if(s.charAt(i)=='{'||s.charAt(i)=='['||s.charAt(i)=='(')
            {
                st.push(s.charAt(i));
            }
                                  
                                  
            else{
                 if(stack.isEmpty())
                 {
                   return "no";
                   }
                     else{
                          char pop_val=stack.pop();
                          if (s.charAt(i)=='}' && pop_val != '{'){
                                  return "NO";}
                        else  if (s.charAt(i)==')' && pop_val != '('){
                                  return "NO";}
                        else  if (s.charAt(i)==']' && pop_val != '['){
                                  return "NO";}
                                  
                                  
            }
                 }
                       }
                                  
                 if(stack.isEmpty())
                  {
                    return "YES";
                   }
                   else
                    {
                    return "NO";
                     }
