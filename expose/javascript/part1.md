1. Line 9 prints 'values added: 20' since add is true, the if block runs and result is declared, then set to 20 (10 + 10). Line 9 logs in the console 'values added: ', result, which results in 'values added: 20' being printed.

2. Line 13 prints 'final result: 20' following the same logic from question 1, but line 13 is outside of the if block and logs in the console 'final result: ', result.

3. You should not use **var** because when a variable is declared with **var**, it is either function-scoped or global-scoped making them visible through blocks. When a **var** is declared, it is processed at the start of the function or start of script if it is global, no matter what line it is in the code. This can become a problem because it can increase the chance of potential bugs from unintended access or overwrites. It can also make the code harder to read and maintain if the scope of variables isn't explicit.

4. Line 9 prints 'values added: 20' since the console.log is inside of the if block and we are using **let**.

5. Line 13 returns an ReferenceError because result is not defined within that block. Since we are using the **let** declaration, result is only defined within the if(add) block. Therefore, line 13 cannot access the result variable, throwing an error.

6. Line 9 is not executed because an error occurs before it. In line 7, there is an error where we cannot assign result to equal num 1 + num 2 because it was declared as a **const** in line 5, which makes it so that it cannot be reassigned after its initial assignment.

7. Line 13 also is not executed because an error occurs before it in line 7. We have an error where  we cannot assign result = num1 + num 2 because result was declared as a **const** in line 5. Declaring result as a **const** means that it cannot be reassigned after its initial assignment.