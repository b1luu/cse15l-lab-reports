# Lab Report 2

**Part 1: StringServer**

Code: StringServer.java implementation:

```
import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler {
  String s = "";

  public String handleRequest(URI url) {
    if (url.getPath().equals("/")) {
      return s;
    }
    else{
      System.out.println("Path: " + url.getPath());
      if (url.getPath().contains("/add-message")){
        String[] parameters = url.getQuery().split("=");
        s = parameters[1];
        return s;
      }
    }
    return "404 Not Found!";
  }
}

class StringServer {
  public static void main(String[] args) throws IOException {
    if (args.length == 0) {
      System.out.println("Missing port number! Try any number between 1024 to 49151");
      return;
    }
    int port = Integer.parseInt(args[0]);
    Server.start(port, new Handler());
  }
}
```



---


**Screenshot for Code with Descriptions:**

![Screenshot 2023-05-10 182916](https://github.com/b1luu/cse15l-lab-reports/assets/120772535/65c2f6a0-b949-4061-ad66-504b8b8cb3ab)

*Description*
* The handleRequest method was called when running `/add-message?s=hello`
* The relevant argument is url
* Values of each field used in method:
  - field **s** is considered the string variable
  - field **parameter** is part of the url before splitting the argument

---

![Screenshot 2023-05-10 185125](https://github.com/b1luu/cse15l-lab-reports/assets/120772535/bdd0c673-0742-45ec-994a-d64a9730803d)

*Description*
* The handleRequest method was called when running `/add-message?s=How are you`
* The relevant argument is url
* Values of each field used in method:
  - field **s** is considered the string variable
  - field **parameter** is part of the url before splitting the argument

>**NOTE**: In the process of adding the message "How are you", I wasn't particular sure how to save `/add-message?s=Hello`. As a result, I was just able to get `How are you` instead of the described `Hello` on the first line followed by `How are you` below. 

---


**Part 2: Debugging Procedure**




Code involved with Lab 3 that we are choosing to debug: `ListExamples.java`

```
static void reverseInPlace(int[] arr) {
  for(int i = 0; i<arr.length; i += 1) {
    arr[i] = arr[arr.length - i - 1];
  }
}
```


Failure Inducing Input:


```
@Test
public void testReverse() {
int[] intList = {10,9,8};
ArrayExamples.reverseInPlace(intList);
asseryArrayEquals(new int[] = {8,9,10}, intList);

```


Non-Failing Inducing Input:


```
@Test
public void testReverse() {
int[] intList = {1};
ArrayExamples.reverseInPlace(intList);
asseryArrayEquals(new int[] = {1}, intList);

```



Fixed Code:


```

static void reverseInPlace(int[] arr) {
      for(int i = 0; i < arr.length/2; i += 1) {
        int newArr = arr[i];
        arr[i] = arr[arr.length - i - 1];
        arr[arr.length - i - 1] = newArr;
      }
    }

```


Original Code:


```
 static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
```


Symptom:

<img width="1423" alt="Screenshot_2023-05-10_at_9 43 33_PM" src="https://github.com/b1luu/cse15l-lab-reports/assets/120772535/d719d91a-f6e8-4733-a51e-1833c05901b3">




*Description*
We needed to create a dummy variable in order to reverse the list properly. We went through the list twice, so divided the for loop iteration in half fixes the problem as well. This way, we can properly traverse through and get the result of reversing the list as desired.

---







**Part 3: Final Thoughts and Reflection**


Reflecting through my process of going through Lab 2, I became increasingly aware of understanding the difference between local device and cloud servers. I appreciate the amount of ease developers have made accessing websites, keeping websites secure, and networked smoothly as there is definately a learning curve towards web development and generated curiousity to how links and networking works. 
