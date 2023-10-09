# Basics of Terminal Commands

## `cd` is short for “current directory”

1. When you type `cd` into the terminal without arguments, your working directory is changed to the root directory.
   > The output of this command is not an error because changing your working directory to the root directory is the default action of `cd`.
    - In the below example, the working directory is `lecture/messages`. When cd is entered without any arguments, the working directory is changed to the root directory.

![Image](https://cdn.discordapp.com/attachments/1065014704986128404/1160764165552603206/Untitled.png?ex=6535d8df&is=652363df&hm=ff2adfd09cc95070932620ec410149c2ba0c6b81fb66fa5ab0f6888393623ce4&)

2. When you type `cd` into the terminal with the path to another *directory*, you change your working directory to the one listed in the new pathname.
    > The output of this command is not an error because you successfully changed directories to the one specified by the pathname.
    - In the below example, the working directory is the root directory. When `cd lecture1/messages` is entered into the terminal, the working directory is  changed to `lecture1/messages`

![Image](https://cdn.discordapp.com/attachments/1065014704986128404/1160764475465535518/Untitled.png?ex=6535d928&is=65236428&hm=e3628beca654ed421d8391e5959a017092153ef3df8ad2af29df72f83a1e1421&)

3. When you type `cd` into the terminal with the path to a *file*, you get an error saying that you cannot use `cd` on something that is **not** a directory.
    > The output of this command is an error because `cd` can only have a directory as the argument.
    - In the below example, the working directory is the root directory. The terminal prints out an error saying that changing the directory to
   ```
    lecture1/[Hello.java](http://Hello.java)
   ```
    cannot be done because `Hello.java` is not a directory.

![Image](https://cdn.discordapp.com/attachments/1065014704986128404/1160764587730292746/Untitled.png?ex=6535d943&is=65236443&hm=86bb5759a06ed003bba5812b285ca4908d2463cbeb8cc8f3e22f2d210a9a2a49&)

---

## `ls` is short for “list”

1. When use the command `ls` without arguments, the terminal prints back the conents of the working directory.
    > The output of this command is not an error because listing out the contents of a directory is the intended result of using `ls`. 
    - In the below example, the working directory is `lecture1`.

![Image](https://cdn.discordapp.com/attachments/1065014704986128404/1160764704331927632/Untitled.png?ex=6535d95f&is=6523645f&hm=4d8a5808dda275b33490436d786c272e6c967bd05ad55d38e83e532e8ffbb8f3&)

2. When you use the command `ls` with the path to a *directory* as an argument, the terminal prints back the filenames of the files in the directory.
    > The output of this command is not an error because listing out the contents of a directory is the intended result of using `ls`.
    - In the below example, the working directory is `lecture1`, and the terminal lists out the files in `lecture1/messages`.

![Image](https://cdn.discordapp.com/attachments/1065014704986128404/1160764849920426165/Untitled.png?ex=6535d982&is=65236482&hm=88c13854602638292e9d0cec6c4d958bfe3aa161dc77e60febd344b381fa1dc8&)

3. When you use the command `ls` with the path to a ****file****, the terminal returns the pathname of that file.
    > The output of this command is not an error because `ls` lists both the contents of directories and details about files.
    - In the below example, the working directory is `lecture1`, and the terminal returns the pathname of the file.

![Image](https://cdn.discordapp.com/attachments/1065014704986128404/1160765026777444352/Untitled.png?ex=6535d9ac&is=652364ac&hm=14c5413ff3b5999b18afeae9a930f87edaf68241590fb244f9052f4c76008861&)

---

## `cat` is short for “concatenate”

1. When you use the command `cat` without any arguments, the terminal will copy your standard input to standard output. Once finished, you can press CTRL + D to end the `cat` command.
    > The output of this command is not an error because copying the standard input to output is one of the intended uses of `cat`.
    - In the below example, the working directory is `lecture1`, and the terminal copies your input `kjhkjh` into the standard output.
    
    ![Image](https://cdn.discordapp.com/attachments/1065014704986128404/1160765117642842182/Untitled.png?ex=6535d9c2&is=652364c2&hm=1fbed95ebf2c1d5a83783b84500b73ca17284cf7f1cd4bf6e38d754568c51dee&)
    

3. When you use the command `cat` with the path to a *************directory************* as the argument, the program will give an error saying that the argument in your command is a directory.
    > The output of this command is an error because `cat` is mainly used to read and/or write files, not directories.
    - In the below example, the working directory is `lecture1`, and the terminal sees that the argument `lecture1/messages` is a directory and gives an error.

![Image](https://cdn.discordapp.com/attachments/1065014704986128404/1160765226610872330/Untitled.png?ex=6535d9db&is=652364db&hm=5ed61a2485623c026d1ea0b209985c64f10e0d8fad8b3c1c0556fbb0f88d2358&)

3. When you use the command `cat` with the path to a ****file**** as the argument, the contents of that file are printed.
    > The output of this command is not an error because the command `cat` is used to read and/or write files.
    - In the below example, `lecture1/[Hello.java](http://Hello.java)` is used as the argument and the contents of `Hello.java` are printed out.

![Image](https://cdn.discordapp.com/attachments/1065014704986128404/1160765301646970911/Untitled.png?ex=6535d9ed&is=652364ed&hm=a4cb258e67744101a5bf5e6cd16a7b119b4bbacd6ddf642802567bf171466549&)
