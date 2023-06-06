# Lab Report 5: 

## Part 1: Debugging Scenario

## Student Post: 

### **What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?**

I am using Windows 10 as my operating system, VSCode for my editor, and google chrome as my browser. 


### **Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.**
Code Being Addressed:

```
VAR=1

if [[ 1 -eq $VAR & 100 -ne $VAR ]]
then
  echo "1"
else
  echo "0"
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
VAR=1

if [[ 1 -eq $VAR]]
then
  echo "1"
else
  echo "0"
fi

```


