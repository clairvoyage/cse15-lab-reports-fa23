# Basics of Terminal Commands

## `cd` is short for “current directory”

1. When you type `cd` into the terminal without arguments, your working directory is changed to the root directory. The output of this command is not an error because changing your working directory to the root directory is the default action of `cd`.
    - In the below example, the working directory is `lecture/messages`. When cd is entered without any arguments, the working directory is changed to the root directory.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/52907341-036d-4dee-8616-6ffddef6bdad/a2362485-1d30-4625-97bf-e919742656e1/Untitled.png)

1. When you type `cd` into the terminal with the path to another *directory*, you change your working directory to the one listed in the new pathname. The output of this command is not an error because you successfully changed directories to the one specified by the pathname.
    - In the below example, the working directory is the root directory. When `cd lecture1/messages` is entered into the terminal, the working directory is  changed to `lecture1/messages`

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/52907341-036d-4dee-8616-6ffddef6bdad/ae8c44d3-d10d-4943-95b5-b3ed7c3c85f9/Untitled.png)

1. When you type `cd` into the terminal with the path to a *file*, you get an error saying that you cannot use `cd` on something that is **not** a directory. 
    - In the below example, the working directory is the root directory. The terminal prints out an error saying that changing the directory to `lecture1/[Hello.java](http://Hello.java)` cannot be done because `Hello.java` is not a directory.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/52907341-036d-4dee-8616-6ffddef6bdad/20e94d6d-4356-44a4-874c-6bb470ac8c72/Untitled.png)

---

## `ls` is short for “list”

1. When use the command `ls` without arguments, the terminal prints back the conents of the working directory. The output of this command is not an error because listing out the contents of a directory is the intended result of using `ls`. 
    - In the below example, the working directory is `lecture1`.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/52907341-036d-4dee-8616-6ffddef6bdad/f7104df4-96d9-4c13-a925-b796b409e8a2/Untitled.png)

1. When you use the command `ls` with the path to a *directory* as an argument, the terminal prints back the filenames of the files in the directory. The output of this command is not an error because listing out the contents of a directory is the intended result of using `ls`.
    - In the below example, the working directory is `lecture1`, and the terminal lists out the files in `lecture1/messages`.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/52907341-036d-4dee-8616-6ffddef6bdad/9f14880a-e49e-4cf1-a431-726cb9380ae4/Untitled.png)

1. When you use the command `ls` with the path to a ****file****, the terminal returns the pathname of that file. The output of this command is not an error because `ls` lists both the contents of directories and details about files.
    - In the below example, the working directory is `lecture1`, and the terminal returns the pathname of the file.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/52907341-036d-4dee-8616-6ffddef6bdad/6d420264-fe64-4a05-9008-ec99576925e7/Untitled.png)

---

## `cat` is short for “concatenate”

1. When you use the command `cat` without any arguments, the terminal will copy your standard input to standard output. Once finished, you can press CTRL + D to end the `cat` command. The output of this command is not an error because copying the standard input to output is one of the intended uses of `cat`.
    - In the below example, the working directory is `lecture1`, and the terminal copies your input `kjhkjh` into the standard output.
    
    ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/52907341-036d-4dee-8616-6ffddef6bdad/fa65de08-8126-456c-8b46-1b4e5b9d59f9/Untitled.png)
    

1. When you use the command `cat` with the path to a *************directory************* as the argument, the program will give an error saying that the argument in your command is a directory. The output of this command is an error because `cat` is mainly used to read and/or write files, not directories.
    - In the below example, the working directory is `lecture1`, and the terminal sees that the argument `lecture1/messages` is a directory and gives an error.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/52907341-036d-4dee-8616-6ffddef6bdad/eb7e3bd1-c1c2-449f-bcea-8c50d7996b59/Untitled.png)

1. When you use the command `cat` with the path to a ****file**** as the argument, the contents of that file are printed. The output of this command is not an error because the command `cat` is used to read and/or write files.
    - In the below example, `lecture1/[Hello.java](http://Hello.java)` is used as the argument and the contents of `Hello.java` are printed out.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/52907341-036d-4dee-8616-6ffddef6bdad/b9d2bf41-1191-4b55-a090-f406e4cadb26/Untitled.png)
