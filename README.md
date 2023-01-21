Create a cpp file from code blocks.
Copy this full code
and run the following expression
  
  ((a+b-c)*d^e^f)/g
  
  
  
  
  
**Algorithm that works behind it**
1)An infix expression and stack are passing as parameters from the driver class(parameters of infixToPostfix function)
2)The function is checking the whole infix expression into two ways. 
   1)By scanning operands
   2)By scanning operators
3)By checking operands from (a-z) & from (A-Z)
 this is adding into the string type variable (postfix)
4)After that,it's checking the parenthesis whether it is '(' or ')'.
  If it is opening,then it's pushing to the stack & if it is the ')'
then it's adding the elements from the top of the stack into the postfix.
5)In the second part it's cehcking the operator.
  Note:isOperator() is a user defined function where it's checking the operator whether
    it's ('+' or '-' or '*' or '/' or '^')
  6)If stack is empty,then easily it's pushing into the stack
    other wise it's checking the precedence of the operator through another user defined function.
    And only adding into the postfix when it get's less than or equal precedence from the stack.
    
    and finally rest of the elements are adding into the postfix.
