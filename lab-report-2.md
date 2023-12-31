# **Lab Report 2: Blog post**
## Part 1
### Code:

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

### Screenshot 1:

Which methods in your code are called?

- handleRequest

What are the relevant arguments to those methods, and the values of any relevant fields of the class?

- relevant argument: URI url
- relevant fields to class: String str, int strCount

How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.

- URI url changes when /add-message is added to the end of the url. Here, `add-message?s=Hello` was added.
- By default, String str = "Try typing '/add-message?s=' and your own message after the address and see what happens!" After doing the add-message request, the message String is appended to String str. In this example, the String “Hello” is appended to str.
- int strCount is incremented to show the current number of the message. In this case, `strCount = 0` incremented to `strCount = 1`.

![image](https://media.discordapp.net/attachments/1165737971237011628/1165738113902071938/Screenshot_2023-10-21_at_15.png?ex=6547f138&is=65357c38&hm=17b23587ecf0ae1afb5f491d948efce1ae18afcaf01116f56ac1d3ee783998a8&=&width=1480&height=832)

### Screenshot 2

Which methods in your code are called?

- handleRequest

What are the relevant arguments to those methods, and the values of any relevant fields of the class?

- relevant argument: URI url
- relevant fields to class: String str, int strCount

How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.

- URI url changes when /add-message is added to the end of the url. In this case, `/add-message?s="How are you?"` is added to the url.
- By default, String str = "Try typing '/add-message?s=' and your own message after the address and see what happens!" After doing the add-message request, the message String is appended to String str. In this example, the String “How are you?” is appended to str.
- int strCount is incremented to show the current number of the message. It went from `strCount = 1` to `strCount = 2`.

![image](https://media.discordapp.net/attachments/1165737971237011628/1165738146709901403/Screenshot_2023-10-21_at_15.png?ex=6547f140&is=65357c40&hm=484dcdd50ccab0af1358bcd928874db486f69ecc1b84c48471fdd09ba76e6f31&=&width=1480&height=832)

## Part 2

### Path to private key:
The private key is id_rsa, located at `/Users/merlin/.ssh/id_rsa` in my own computer.
![image](https://media.discordapp.net/attachments/1165737971237011628/1165747714265448498/image.png?ex=6547fa29&is=65358529&hm=fc17228fa360ed39396ae2835015fcf9f4700420164550aa65c121eed38f4fba&=&width=1480&height=152)

### Path to public key:
The public key is id_rsa.pub, located at `~/.ssh/id_rsa.pub` in `ieng6`.
![image](https://media.discordapp.net/attachments/1165737971237011628/1165747403505283233/image.png?ex=6547f9df&is=653584df&hm=0348f77db64416917e5ab7cb7d9a837f945268c8e29c410330d602e865cb1929&=&width=1480&height=142)

### Logging into ieng6 without password:

![image](https://media.discordapp.net/attachments/1165737971237011628/1165738215957872670/Untitled.png?ex=6547f151&is=65357c51&hm=afc0802aad10788c86e35bc44e4aa82dfb2f527681bad240e41f72cb02514230&=&width=1480&height=660)

## Part 3

Something I learned from the Week 3 lab was how to create a local server and edit it. I learned that to make any edits to the handler show up on the server's web page, you have to close the server and compile and run the server files again.




