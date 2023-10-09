# Basics of Terminal Commands

## `cd` is short for “current directory”

1. When you type `cd` into the terminal without arguments, your working directory is changed to the root directory.
   > The output of this command is not an error because changing your working directory to the root directory is the default action of `cd`.   
   - In the below example, the working directory is `lecture1/messages`. When cd is entered without any arguments (that is, without any text after `cd`), the working directory is changed to the root directory, which is `lecture1`.   

   ![Image](https://cdn.discordapp.com/attachments/1065014704986128404/1160764165552603206/Untitled.png?ex=6535d8df&is=652363df&hm=ff2adfd09cc95070932620ec410149c2ba0c6b81fb66fa5ab0f6888393623ce4&) 

2. When you type `cd` into the terminal with the path to another *directory*, you change your working directory to the one listed in the new pathname.
   > The output of this command is not an error because you successfully changed directories to the one specified by the pathname.
   - In the below example, the working directory is the root directory, `lecture1`. When `cd lecture1/messages` is entered into the terminal, the working directory is  changed to `lecture1/messages`.
   
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
   - In the below example, the working directory is `lecture1`, and the terminal lists out the files in `lecture1/messages`. The files in `lecture1/messages` are: `en-us.txt`, `es-mx.txt`, and `zh-cn.txt`.
![Image](https://cdn.discordapp.com/attachments/1065014704986128404/1160764849920426165/Untitled.png?ex=6535d982&is=65236482&hm=88c13854602638292e9d0cec6c4d958bfe3aa161dc77e60febd344b381fa1dc8&)

3. When you use the command `ls` with the path to a **file**, the terminal returns the pathname of that file.
   > The output of this command is not an error because `ls` lists both the contents of directories and details about files.
   - In the below example, the working directory is `lecture1`, and the terminal returns the pathname of the file `lecture1/Hello.java`.

![Image](https://cdn.discordapp.com/attachments/1065014704986128404/1160765026777444352/Untitled.png?ex=6535d9ac&is=652364ac&hm=14c5413ff3b5999b18afeae9a930f87edaf68241590fb244f9052f4c76008861&)

---

## `cat` is short for “concatenate”

1. e
2. e
3. e
   
