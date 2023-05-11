# Lab Report 2

** Part 1: **

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


![Screenshot 2023-05-10 182916](https://github.com/b1luu/cse15l-lab-reports/assets/120772535/65c2f6a0-b949-4061-ad66-504b8b8cb3ab)



