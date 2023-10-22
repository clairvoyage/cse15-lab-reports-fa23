code:

```java
// Authors: Joe Gibbs Politz and Merlin Ho

import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler {
    // The one bit of state on the server: a number that will be manipulated by
    // various requests.
    String str = "Try typing '/add-message?s=' and your own message after the address"
            + " and see what happens!";
    int strCount = 0;

    public String handleRequest(URI url) {
        if (url.getPath().equals("/")) {
            return String.format(str);
        } else {
            if (url.getPath().contains("/add-message")) {
                strCount++;
                String[] parameters = url.getQuery().split("=");
                str = str + "\n" + strCount + ". " + parameters[1];
                return str;
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

### screenshot 1:

Which methods in your code are called?

- handleRequest

What are the relevant arguments to those methods, and the values of any relevant fields of the class?

- relevant argument: URI url
- relevant fields to class: String str, int strCount

How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.

- URI url changes when /add-message is added to the end of the url.
- By default, String str = "Try typing '/add-message?s=' and your own message after the address and see what happens!" After doing the add-message request, the message String is appended to String str. In this example, the String “Hello” is appended to str.
- int strCount is incremented to show the current number of the message.

![Screenshot 2023-10-21 at 15.26.54.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/52907341-036d-4dee-8616-6ffddef6bdad/dacb665a-47f0-47bc-ab10-14fc6b517997/Screenshot_2023-10-21_at_15.26.54.png)

### screenshot 2

Which methods in your code are called?

- handleRequest

What are the relevant arguments to those methods, and the values of any relevant fields of the class?

- relevant argument: URI url
- relevant fields to class: String str, int strCount

How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.

- URI url changes when /add-message is added to the end of the url.
- By default, String str = "Try typing '/add-message?s=' and your own message after the address and see what happens!" After doing the add-message request, the message String is appended to String str. In this example, the String “Hello” is appended to str.
- int strCount is incremented to show the current number of the message.

![Screenshot 2023-10-21 at 15.27.37.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/52907341-036d-4dee-8616-6ffddef6bdad/365efacd-cd1a-4d32-b442-de2d017d597e/Screenshot_2023-10-21_at_15.27.37.png)

im suffering

/.ssh/authorized_keys

jesus that took way more effort than i wanted it to

basically in the instructions for the lab they give you the path the path to the public and private key already and you can just cd to there 😟

# part 2

path to private key:

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/52907341-036d-4dee-8616-6ffddef6bdad/01bb2938-9083-4f54-93db-c2c7e6d71efd/Untitled.png)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/52907341-036d-4dee-8616-6ffddef6bdad/0bcc0388-f1e2-4905-b4b8-5d6add51d870/Untitled.png)

path to public key:

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/52907341-036d-4dee-8616-6ffddef6bdad/0606cb8a-f4a9-47a6-9168-d716ba821aa0/Untitled.png)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/52907341-036d-4dee-8616-6ffddef6bdad/fa1f19c1-5c2a-4352-97a6-8bd9d5e86297/Untitled.png)

logging into ieng6 without password:

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/52907341-036d-4dee-8616-6ffddef6bdad/26da12dd-ec02-4812-97c5-09292c69606e/Untitled.png)
