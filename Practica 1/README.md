# 7_semester
## Цель работы

1. Познакомиться с языком R посредством библиотеки  swirl.

## Исходные данные

1. Rstudio.

## План

1. Установить библиотеку swirl.
2. Пройти 4 учебных задания.
3. Оформить отчет.

## Описание шагов

1. Установка библиотеки swirl.
```
install.packages("swirl")
```
2. Запускаем библиотеку. 
```
library(swirl)
swirl()
```
3. Основные блоки программирования на языке R
 In its simplest form, R can be used as an interactive calculator. Type 5 + 7 and press Enter

```{r}
5+7
```

    | Type x <- 5 + 7. It's important to include a single space on each side of the assignment operator, but do NOT put a space between the
    | `<` and the `-` that form the arrow.

```{r}
x<-5+7
```

    | Type y <- x - 3 and press Enter. Whether you use x - 3 or x-3 is personal preference, but it's good habit to include a space on either
    | side of the assignment operator.

```{r}
y<- x-3
```

    | The easiest way to create a vector is with the c() function, which stands for 'concatenate' or 'combine'. To create a vector containing
    | the numbers 1.1, 9, and 3.14, type c(1.1, 9, 3.14). Try it now and store the result in a variable called z.

```{r}
z<- c(1.1,9,3.14)
```

    | Anytime you have questions about a particular function, you can access R's built-in help files via the `?` command. For example, if you
    | want more information on the c() function, type ?c without the parentheses that normally follow a function name. Give it a try.

```{r}
?c
```

    | You can combine vectors to make a new vector. Create a new vector that contains z, 555, then z again in that order. Don't assign this
    | vector to a new variable, so that we can just see the result immediately.

```{r}
c(z,555,z)
```

    | Numeric vectors can be used in arithmetic expressions. Type the following to see what happens: z * 2 + 100

```{r}
z*2+100
```

    | Take the square root of z - 1 and assign it to a new variable called my_sqrt.

```{r}
my_sqrt<-sqrt(z-1)
```

    | Assign the result of sqrt(z - 1) to a variable called my_sqrt.

```{r}
my_sqrt<-sqrt(z-1)
```

    | Before we view the contents of the my_sqrt variable, what do you think it contains?

    1: a vector of length 3
    2: a single number (i.e a vector of length 1)
    3: a vector of length 0 (i.e. an empty vector)

    Выбор:1

    | Now, create a new variable called my_div that gets the value of z divided by my_sqrt.

```{r}
my_div<-z/my_sqrt
```

    | Which statement do you think is true?

    1: my_div is undefined
    2: my_div is a single number (i.e a vector of length 1)
    3: The first element of my_div is equal to the first element of z divided by the first element of my_sqrt, and so on...

    Выбор:3

    | Keep up the great work!

    | To see another example of how this vector 'recycling' works, try adding c(1, 2, 3, 4) and c(0, 10). Don't worry about saving the result
    | in a new variable.

```{r}
c(1,2,3,4)+c(0,10)
```

    | Try c(1, 2, 3, 4) + c(0, 10, 100) for an example

```{r}
c(1, 2, 3, 4) + c(0, 10, 100)
```

    | Type c(1, 2, 3, 4) + c(0, 10, 100) to see how R handles adding two vectors, when the shorter vector's length does not divide evenly into
    | the longer vector's length. Don't worry about assigning the result to a variable.

    > c(1, 2, 3, 4) + c(0, 10, 100)
    [1]   1  12 103   4
    Warning message:
    In c(1, 2, 3, 4) + c(0, 10, 100) :
      longer object length is not a multiple of shorter object length

    | Keep up the great work!

    | In many programming environments, the up arrow will cycle through previous commands. Try hitting the up arrow on your keyboard until you
    | get to this command (z * 2 + 100), then change 100 to 1000 and hit Enter. If the up arrow doesn't work for you, just type the corrected
    | command.

```{r}
z*2+1000
```

    | You can type the first two letters of the variable name, then hit the Tab key (possibly more than once). Most programming environments
    | will provide a list of variables that you've created that begin with 'my'. This is called auto-completion and can be quite handy when you
    | have many variables in your workspace. Give it a try. (If auto-completion doesn't work for you, just type my_div and press Enter.)

    > 
    > my_div
    [1] 3.478505 3.181981 2.146460

    | You nailed it! Good job!

      |======================================================| 100%
    | Would you like to receive credit for completing this course on Coursera.org?

<img width="636" alt="Снимок экрана 2023-10-01 в 15 25 53" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/c8613a00-5772-4ca8-b11f-b5dda1f59d4e">
<img width="631" alt="Снимок экрана 2023-10-01 в 15 35 56" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/50aeb7cf-1500-4d87-a3cc-af118c33a332">
<img width="638" alt="Снимок экрана 2023-10-01 в 15 36 18" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/1c6f4467-f5a8-46a8-ad15-79e71d80e492">
<img width="638" alt="Снимок экрана 2023-10-01 в 15 37 14" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/eb5005a1-5762-4340-ae80-db509ad76bf2">
<img width="635" alt="Снимок экрана 2023-10-01 в 15 38 33" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/1da115b5-a509-4b22-a446-45161abd7e4c">
<img width="638" alt="Снимок экрана 2023-10-01 в 15 39 01" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/ce9ac145-04a7-4f7a-bdcf-4bed77a86196">
<img width="635" alt="Снимок экрана 2023-10-01 в 15 40 55" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/821e8f4e-8da4-4b08-b8c4-d4412205f118">
<img width="625" alt="Снимок экрана 2023-10-01 в 15 41 39" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/55fc41f2-2d07-487b-bbc9-d4aeafe79f50">
<img width="642" alt="Снимок экрана 2023-10-01 в 15 42 38" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/4a53347b-a753-402d-819b-68067e2f3248">
<img width="667" alt="Снимок экрана 2023-10-01 в 15 44 34" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/eb98e791-9335-43db-b442-e053c6f16750">
<img width="644" alt="Снимок экрана 2023-10-01 в 15 45 38" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/3e0b6b65-d47f-4d62-8fd8-8768d62f14d4">
<img width="631" alt="Снимок экрана 2023-10-01 в 15 46 11" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/fd806f4a-f66c-4482-a3de-a0444b2041fb">
<img width="622" alt="Снимок экрана 2023-10-01 в 15 47 22" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/61b91a63-0d07-4ef1-ae60-df3e1d0b17c9">


4. Выполяем второе учебное задание Workspace and Files.
    Access information about the file "mytest.R" by using
    | file.info().

file.info("mytest.R")

    | Determine which directory your R session is using as its current working directory using getwd().

getwd()

    [1] "/User/anna"

    | Now take a look at objects that are in your workspace using ls().

ls()

    [1] "my_div"  "my_sqrt" "v"       "x"       "y"       "z"

    Assign 9 to x using x <- 9.

```{r}
x<-9
```

    | Now take a look at objects that are in your workspace using ls().

ls

     List all the files in your working directory using list.files() or dir().

dir()
 [1] "7_Lab_a"                  "7_Lab_Dima"               "7_Laba"                  
 [4] "Applications (Parallels)" "C++"                      "Desktop"                 
 [7] "Documents"                "Downloads"                "dz_1_koragin"            
[10] "HelloWorld"               "IdeaProjects"             "Koragin_1_DZ"            
[13] "Koragin_1_dz_.cs"         "Lab_7"                    "Laba_7_Katya"            
[16] "Library"                  "mindmap.mm"               "Movies"                  
[19] "Music"                    "Parallels"                "Pictures"                
[22] "primer dla 7 pr"          "Projects"                 "Public"                  
[25] "PycharmProjects"          "R-Studio"                 "testdir"                 
[28] "VirtualBox VMs" 

    | As we go through this lesson, you should be examining the help page for each new function. Check out the help page for list.files with
    | the command ?list.files.

?list.files

args(list.files)

    function (path = ".", pattern = NULL, all.files = FALSE, full.names = FALSE, 
        recursive = FALSE, ignore.case = FALSE, include.dirs = FALSE, 
        no.. = FALSE) 
    NULL

    | Assign the value of the current working directory to a variable called "old.dir".

old.dir \<- getwd()

dir.create("testdir")

     Set your working directory to "testdir" with the setwd() command.

setwd("testdir")

    | Create a file in your working directory called "mytest.R" using the file.create() function.

file.create("mytest.R")

    [1] TRUE

    | This should be the only file in this newly created directory. Let's check this by listing all the files in the current directory.

list.files()

    [1] mytest.R

    Use file.exists("mytest.R") to check that a file exists().

file.exists("mytest.R")

    [1] TRUE

    Access information about the file "mytest.R" by using
    | file.info()

file.info("mytest.R")
         size isdir mode   mtime      ctime              atime    uid gid uname grname
mytest.R  0 FALSE 644    2023-10-01 15:53:36 2023-10-01  15:53:36 501 20   anna staff
    | Nice work!

    | You can use the $ operator --- e.g., file.info("mytest.R")$mode
    | --- to grab specific items

    Change the name of the file "mytest.R" to "mytest2.R" by using file.rename()

file.rename("mytest.R", "mytest2.R")
[1] TRUE

    | Make a copy of "mytest2.R" called "mytest3.R" using file.copy().

file.copy("mytest2.R","mytest3.R")

    | Provide the relative path to the file "mytest3.R" by using file.path().

file.path("mytest3.R")

    You can use file.path to construct file and directory paths that are independent of the operating system your R code is running on. Pass
    | 'folder1' and 'folder2' as arguments to file.path to make a platform-independent pathname.

file.path("folder1", "folder2")
[1] folder1/folder2

    | ?dir.create will show you the docs.

    > ?dir.create

    | Create a directory in the current working directory called "testdir2" and a subdirectory for it called "testdir3", all in one command by
    | using dir.create() and file.path().

dir.create(file.path('testdir2', 'testdir3'), recursive = TRUE)

    | Go back to your original working directory using setwd(). (Recall that we created the variable old.dir with the full path for the orginal
    | working directory at the start of these questions.)

setwd(old.dir)

<img width="629" alt="Снимок экрана 2023-10-01 в 15 48 51" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/db1fed34-de6c-4b25-9df6-5c9e2521103c">
<img width="991" alt="Снимок экрана 2023-10-01 в 15 50 27" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/616843b9-c4c8-4f73-91bc-72e8dc93a8b1">
<img width="640" alt="Снимок экрана 2023-10-01 в 15 51 43" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/b89045a1-7820-40f7-9927-e65eb791dc7a">
<img width="625" alt="Снимок экрана 2023-10-01 в 15 53 12" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/0263642b-5e7d-46be-b0c5-417a292924a2">
<img width="640" alt="Снимок экрана 2023-10-01 в 15 55 00" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/f5c95a21-8ead-49e1-937f-f5440ecb3633">
<img width="637" alt="Снимок экрана 2023-10-01 в 15 56 15" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/ab36d3a2-e717-48d5-a165-69b0cf69727f">
<img width="626" alt="Снимок экрана 2023-10-01 в 16 00 15" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/89e89b1e-b9d8-4b68-bf0a-d3a2d0925989">
<img width="625" alt="Снимок экрана 2023-10-01 в 16 01 18" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/77f4f198-ca48-452b-a46b-19e407327fe9">


5. Выполняем третье учебное задание Sequences of Numbers.
   | The simplest way to create a sequence of numbers in R is by using the `:` operator. Type 1:20 to see how it works.

```{r}
1:20
[1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20
```

    | That gave us every integer between (and including) 1 and 20. We could also use it to create a sequence of real numbers. For example, try
    | pi:10.

```{r}
pi:10
[1] 3.141593 4.141593 5.141593 6.141593 7.141593 8.141593 9.141593
```

    | What happens if we do 15:1? Give it a try to find out

```{r}
15:1
 [1] 15 14 13 12 11 10  9  8  7  6  5  4  3  2  1
```

    | Pull up the documentation for `:` now.

    ?':'

    The most basic use of seq() does exactly the same thing as the `:` operator. Try seq(1, 20) to see this.

```{r}
seq(1, 20)
[1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20
```

    | This gives us the same output as 1:20. However, let's say that instead we want a vector of numbers ranging from 0 to 10, incremented by
    | 0.5. seq(0, 10, by=0.5) does just that. Try it out.

```{r}
seq(0, 10, by=0.5)
 [1]  0.0  0.5  1.0  1.5  2.0  2.5  3.0  3.5  4.0  4.5  5.0  5.5  6.0  6.5  7.0  7.5  8.0  8.5
[19]  9.0  9.5 10.0
```

    | Or maybe we don't care what the increment is and we just want a sequence of 30 numbers between 5 and 10. seq(5, 10, length=30) does the
    | trick. Give it a shot now and store the result in a new variable called my_seq.

```{r}
my_seq <- seq(5, 10, length=30)
```

    | To confirm that my_seq has length 30, we can use the length() function. Try it now.

```{r}
length(my_seq)
 [1] 30
```

    | There are several ways we could do this. One possibility is to combine the `:` operator and the length() function like this:
    | 1:length(my_seq). Give that a try.

```{r}
1:length(my_seq)
[1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30
```

```{r}
seq(along.with = my_seq)
[1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30
```

    | However, as is the case with many common tasks, R has a separate built-in function for this purpose called seq_along(). Type
    | seq_along(my_seq) to see it in action.

```{r}
seq_along(my_seq)
[1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30
```

    | If we're interested in creating a vector that contains 40 zeros, we can use rep(0, times = 40). Try it out.

```{r}
rep(0, times = 40)
[1] 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0
```

    | If instead we want our vector to contain 10 repetitions of the vector (0, 1, 2), we can do rep(c(0, 1, 2), times = 10). Go ahead.

```{r}
rep(c(0, 1, 2), times = 10)
[1] 0 1 2 0 1 2 0 1 2 0 1 2 0 1 2 0 1 2 0 1 2 0 1 2 0 1 2 0 1 2
```

    | Finally, let's say that rather than repeating the vector (0, 1, 2) over and over again, we want our vector to contain 10 zeros, then 10
    | ones, then 10 twos. We can do this with the `each` argument. Try rep(c(0, 1, 2), each = 10).

```{r}
rep(c(0, 1, 2), each = 10)
[1] 0 0 0 0 0 0 0 0 0 0 1 1 1 1 1 1 1 1 1 1 2 2 2 2 2 2 2 2 2 2
```
<img width="627" alt="Снимок экрана 2023-10-01 в 16 02 15" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/396b1da6-7d88-45f7-94b1-f9f101ba7f31">
<img width="634" alt="Снимок экрана 2023-10-01 в 16 02 51" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/22455376-595f-4956-b531-6d50e3dd9f5f">
<img width="622" alt="Снимок экрана 2023-10-01 в 16 03 26" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/1c98e97c-55b0-462c-b902-4aa08d937de3">
<img width="636" alt="Снимок экрана 2023-10-01 в 16 04 10" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/51939068-6079-4d49-8b75-b2d36c0cece0">
<img width="633" alt="Снимок экрана 2023-10-01 в 16 05 13" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/493027c6-7c89-40ae-a9bf-6668e4a9fe82">


6. Выполняем четвертое учебное задание Vectors.
```{r}
> num_vect <- c(0.5, 55, -10, 6)
```

```{r}
> tf <- num_vect < 1
```

```{r}
> tf
[1]  TRUE FALSE  TRUE FALSE
```

```{r}
> num_vect >= 6
[1] FALSE  TRUE FALSE  TRUE
```

```{r}
(3 > 5) & (4 == 4)
FALSE & TRUE = FALSE
1: FALSE
2: TRUE

Selection: 1
```

```{r}
(TRUE == TRUE) | (TRUE == FALSE)
TRUE | FALSE = TRUE
1: FALSE
2: TRUE

Selection: 2
```

```{r}
((111 >= 111) | !(TRUE)) & ((4 + 1) == 5)
(TRUE | FALSE) & TRUE
TRUE & TRUE
1: FALSE
2: TRUE

Selection: 1
```

```{r}
> my_char <- c("My", "name", "is")
```

```{r}
> my_char
[1] "My"   "name" "is" 
```

```{r}
> paste(my_char, collapse = " ")
[1] "My name is"
```

```{r}
> my_name <- c(my_char, "Katya")
```

```{r}
> my_name
[1] "My"     "name"   "is"     "Anna"
```

```{r}
> paste(my_name, collapse = " ")
[1] "My name is Anna"
```

```{r}
> paste("Hello", "world!", sep = " ")
[1] "Hello world!"
```

```{r}
> paste(1:3, c("X","Y","Z"), sep = "")
[1] "1X" "2Y" "3Z"
```

```{r}
> paste(LETTERS, 1:4, sep = "-")
 [1] "A-1" "B-2" "C-3" "D-4" "E-1" "F-2" "G-3" "H-4" "I-1" "J-2" "K-3" "L-4"
[13] "M-1" "N-2" "O-3" "P-4" "Q-1" "R-2" "S-3" "T-4" "U-1" "V-2" "W-3" "X-4"
[25] "Y-1" "Z-2"

<img width="630" alt="Снимок экрана 2023-10-01 в 16 06 06" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/fb3f09c9-2d01-4cdd-97b8-6fe1aedfb3cd">
<img width="633" alt="Снимок экрана 2023-10-01 в 16 06 44" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/73174a94-ae20-4f74-b1c7-80acbc404484">
<img width="639" alt="Снимок экрана 2023-10-01 в 16 07 21" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/4c87bd68-a3da-4641-b9ac-108f01a93f81">
<img width="645" alt="Снимок экрана 2023-10-01 в 16 08 34" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/43b322fa-65e6-4a75-a0b7-b4aeb6e58c1d">
<img width="630" alt="Снимок экрана 2023-10-01 в 16 09 34" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/792ad21d-f1b8-4527-ac35-b95fa4cf05d5">
<img width="630" alt="Снимок экрана 2023-10-01 в 16 10 11" src="https://github.com/GavrilovaAnna/7_semester/assets/91331145/579fa602-23e4-4c71-bcc8-6f167965d514">


## Оценка результатов

Задача выполнена при помощи приложения RStudio, удалось познакомится с его функционалом и особенностями.

## Вывод
В данное практической работе я познакомилась с основами языка R. Таким образом, я приобрела базовые новыки для работы с языком R.
