[![MIT Licensed][icon-mit]][license]
[![Awesome][icon-awesome]][awesome]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

# Golang Basics Part I

Please complete the courses, tutorials and tasks listed below:

### Theory

1. As any young gopher we start by passing "[Tour of Go](https://tour.golang.org)"
1. Go through 1-7 chapter at [Golangbootcamp](http://www.golangbootcamp.com/book). Check your knowledge with exercizes at the end of 3,4,5,7 chapters.
1. Read Introduction, Formatting, Commentary, Names, Semicolons, Control structures, Functions and Data chapters from [Effective Go](https://golang.org/doc/effective_go.html) article written by go language developers.
1. Read following important articles:

[Learn Go Variables](https://blog.learngoprogramming.com/learn-go-lang-variables-visual-tutorial-and-ebook-9a061d29babe)

[Learn golang typed untyped constants](https://blog.learngoprogramming.com/learn-golang-typed-untyped-constants-70b4df443b61)

[Go Blog: String](https://blog.golang.org/strings)

[Understand go pointers in less than 800 words or your money back](https://dave.cheney.net/2017/04/26/understand-go-pointers-in-less-than-800-words-or-your-money-back)

[Go slices usage and internals](https://blog.golang.org/go-slices-usage-and-internals)

[If a map isn't a reference variable what is it](https://dave.cheney.net/2017/04/30/if-a-map-isnt-a-reference-variable-what-is-it)

[Types System](https://rakyll.org/typesystem/)

[Types Conversations](https://golang.org/ref/spec#Conversions)

[Interface values are valueless](https://www.ardanlabs.com/blog/2018/03/interface-values-are-valueless.html)

[Interface semantics](https://www.ardanlabs.com/blog/2017/07/interface-semantics.html)

[Gotchas of defer](https://blog.learngoprogramming.com/gotchas-of-defer-in-go-1-8d070894cb01)

[Panic & Recover](https://go101.org/article/panic-and-recover-more.html)

[Understanding go panic output](https://joeshaw.org/understanding-go-panic-output/)

### Practical task

1. In your `kottans-backend` folder create folder called `digits`.
1. In `digits` folder create file called `main.go`.
1. Given following string:

```go
const digits =
`
 000
0   0
0   0
0   0
0   0
0   0
 000

  1
1 1
  1
  1
  1
  1
11111

 222
2   2
    2
   2
  2
 2
22222

 333
3   3
    3
  33
    3
3   3
 333

   4
  44
 4 4
4  4
44444
   4
   4

55555
5
5
5555
    5
5   5
 555

 666
6   6
6
6666
6   6
6   6
 666

77777
    7
    7
   7
  7
 7
 7

 888
8   8
8   8
 888
8   8
8   8
 888

 999
9   9
9   9
 9999
    9
9   9
 999
`
```

In `main.go` create write a program that satisfy following [user stories](https://en.wikipedia.org/wiki/User_story):

- As the user, I can take any unsigned integer (`uint`) value to use as argument in `go run main.go <unsigned_integer>` call.
- Using `uint` as input I can get output value as ASCII art in my termanal window. For instance:

`go run main.go 1234567890`

```go
***********************************************************
  1    222   333     4  55555  666  77777  888   999   000
1 1   2   2 3   3   44  5     6   6     7 8   8 9   9 0   0
  1       2     3  4 4  5     6         7 8   8 9   9 0   0
  1      2    33  4  4  5555  6666     7   888   9999 0   0
  1     2       3 44444     5 6   6   7   8   8     9 0   0
  1    2    3   3    4  5   5 6   6  7    8   8 9   9 0   0
11111 22222  333     4   555   666   7     888   999   000
***********************************************************
```

- Note, that asterisk borders are mandatory
- As the user, I can see error message in my terminal if my input is not valid (in case if given more than 1 argument or if 1 argument is not `uint` value).

4. _Optional story_. Add possibily to set custom pixel symbol for your ASCII art via additional command line argument `symbol`. For instance:

`go run main.go -symbol @ 1234567890`

Will output:

```go
***********************************************************
  @    @@@   @@@     @  @@@@@  @@@  @@@@@  @@@   @@@   @@@
@ @   @   @ @   @   @@  @     @   @     @ @   @ @   @ @   @
  @       @     @  @ @  @     @         @ @   @ @   @ @   @
  @      @    @@  @  @  @@@@  @@@@     @   @@@   @@@@ @   @
  @     @       @ @@@@@     @ @   @   @   @   @     @ @   @
  @    @    @   @    @  @   @ @   @  @    @   @ @   @ @   @
@@@@@ @@@@@  @@@     @   @@@   @@@   @     @@@   @@@   @@@
***********************************************************
```

5. Useful links

- [Strings cheatsheet](https://yourbasic.org/golang/string-functions-reference-cheat-sheet/)
- [Os Args Example](https://gobyexample.com/command-line-arguments)

6. In your `kottans-backend` repo `README.md`:
   - add header `## Go basics 1`
   - embed the link to your `main.go` source code file.

##### Code Submission

Save your program in a file. Follow instructions in [this repo](https://github.com/kottans/golang-2019-homeworks) to submit your code.

7. You did lot already! If you honestly finished all the previous steps then go ahead
   and share it with others ???
   post a message in [course channel](https://t.me/joinchat/Dqrdixe1c2K9bXUFBzNWtg):
   `Go Basics 1 ??? #done` and add the link to your repo. **This step is important, as it helps mentors to track your progress!**

## Extra materials

1. [FreeCodeCamp Golang Course](https://www.youtube.com/playlist?list=PLJbE2Yu2zumCe9cO3SIyragJ8pLmVv0z9)
1. [Go By Example](https://gobyexample.com/)
1. [An Introduction to Programming in Go](https://www.golang-book.com/books/intro);
1. [50 ???????????????? Go](https://habr.com/ru/company/mailru/blog/314804/)

## Done?

?????? Go forward to [Memory Management](memory-management.md)

?????? Back to [Contents](../contents.md)

[icon-chat]: https://img.shields.io/badge/chat-on%20telegram-blue.svg
[icon-mit]: https://img.shields.io/badge/license-MIT-blue.svg
[icon-awesome]: https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg
[license]: https://github.com/Kottans/web/blob/master/LICENSE.md
[awesome]: https://github.com/sindresorhus/awesome
