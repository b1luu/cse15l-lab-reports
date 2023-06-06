# Lab Report 5: 

## Part 1: Debugging Scenario

## Student Post: 

### **What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?**

I am using Windows 10 as my operating system, VSCode for my editor, and google chrome as my browser. 


### **Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.**

Java files: `Calculator.java` and `Main.java` in order to run.

`Calculator.java`:
```
public class Calculator {

    public int addNumbers(int num1, int num2) {
        return num1 + num2;
    }


}
```
`Main.java`:
```
public class Main {

    public static void main(String[] args) {
        Calculator calculator = new Calculator();
        int result = calculator.addNumbers(5, 7);
        System.out.println("The sum is: " + result);
    }
}
```

Code Being Addressed: `NeedHelp.sh`

```
filename="Calculator.java"

if [[ -f "$filename"  &  $? -eq 0 ]]
then
  echo "File exists, yay!"
else
  echo "The file does not exist :("
fi

```

In the file **NeedHelp.sh**, I tried to run the command `bash NeedHelp.sh`. I expected to get 1, but got an error here:
> The error can be seen here:

![Screenshot 2023-06-05 185721](https://github.com/b1luu/cse15l-lab-reports/assets/120772535/1e5a6c6f-56e8-4fe3-b397-898c2a73ca0a)

I believe I am correct because there are no logistic errors in my program, but the syntax error in the error message derived from the terminal made me create a different variation of my program and I will provide it in the context below.

### **Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.**

Context:

>Directory of my program: 

![Screenshot 2023-06-05 185721](https://github.com/b1luu/cse15l-lab-reports/assets/120772535/cebec08c-b1f6-4b35-9e23-88c07ff4d893)

As a preface, I made sure I was in the correct directory, made sure my terminal default was bash. My last commands were without the `&` conditional, but I still got an error and I will provide it below:
>Error without `&` in conditional output: 

![Screenshot 2023-06-05 190625](https://github.com/b1luu/cse15l-lab-reports/assets/120772535/33f0a275-e9e0-4caf-bfc2-67ec006c149d)

> Code that caused the failure-inducing output:

```
filename="Calculator.java"

if [[ -f "$filename"]]
then
  echo "File exists, yay!"
else
  echo "The file does not exist :("
fi
```

What is causing this error and what syntax would be needing correction to create a correct implementation?


## TA Response:

Response:

 Java files and program implementation is good--interesting. There seems to be a bug in line #3 in terms of syntax error. If we look at the `If` conditional, shell's `&` conditional is normally represented as `&&` instead of singleton `&`. Also, shell also has `[[` / `]]` grouping specific terms which is different from other languages. Try fixing the syntax for grouping, spacing, and & and run the command `bash NeedHelp.sh`. Here is also a link that provides syntax regarding shell [here](https://www.geeksforgeeks.org/conditional-statements-shell-script/#). Hope this helps! 


## Student Response After Hearing Feedback on TA:

Response:

Thank you. I have updated the code and have noticed the grouping error. I understand that the original error was that line 3 needed to have `]]` and `[[` between the `&` respectively. This is how shell's syntax is made when using `if` conditionals. 

>Correct Output:

![Screenshot 2023-06-05 194444](https://github.com/b1luu/cse15l-lab-reports/assets/120772535/7d32e9fc-e140-4548-9d01-8d1bb2b40343)

>Code with correct output:

filename="Calculator.java"
```
if [[ -f "$filename" ]]  && [[ $? -eq 0 ]]
then
  echo "File exists, yay!"
else
  echo "The file does not exist :("
fi
```



