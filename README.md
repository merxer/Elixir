# 

# Introduction {#introduction}

1. [Installation](#installation)
2. [Interactive mode](#interactive-mode)
3. [Running scripts](#running-scripts)
4. [Asking questions](#asking-questions)

ยินดีต้อนรับ!

ในบทนี้จะสอนเกี่ยวกับพื้นฐานการเขียน Elixir, ประกอบไปด้วย โครงสร้างภาษา, การเขียนโปรแกรมแบบโมดูล, การจัดการต่างๆ เช่นพวก data structures และอื่นๆอีกมากมาย  แต่บทนี้จะเน้นให้สามารถใช้ Interactive shell ของ Elixir ที่เรียกว่า IEx ได้

สิ่งที่ต้องการก่อนเรียน:

* Elixir - Version 1.4.0 หรือใหม่กว่า
* Erlang - Version 18.0 หรือไม่กว่า

มาเริ่มกันเลยดีกว่า!

> ถ้าหากเจอว่ามีตรงใหนผิด สามารถแจ้งเราได้ที่ ,[please report a bug or send a pull request to our issue tracker](https://github.com/elixir-lang/elixir-lang.github.com).

## Installation {#installation}

ถ้าหากตอนนี้ คุณยังไม่มีคอมไพเลอร์ Elixir, ให้ไปดูตัวอย่างการลงได้ที่ [installation page](http://elixir-lang.org/install.html) ถ้าหากลงเสร็จเรียบร้อยแล้ว ลองรันคำสั่ง

`elixir --version`ก็จะได้เลขเวอร์ชั่น ของคอมไพเลอร์ Elixir ออกมา

## Interactive mode {#interactive-mode}

When you install Elixir, you will have three new executables:`iex`,`elixir`and`elixirc`. If you compiled Elixir from source or are using a packaged version, you can find these inside the`bin`directory.

For now, let’s start by running`iex`\(or`iex.bat`if you are on Windows\) which stands for Interactive Elixir. In interactive mode, we can type any Elixir expression and get its result. Let’s warm up with some basic expressions.

Open up`iex`and type the following expressions:

```
Erlang/OTP 19 [erts-8.1] [source] [64-bit] [smp:4:4] [async-threads:10] [hipe] [kernel-poll:false] [dtrace]

Interactive Elixir (1.4.0) - press Ctrl+C to exit (type h() ENTER for help)
iex(1)
>
 40 + 2
42
iex(2)
>
 "hello" 
<
>
 " world"
"hello world"
```

Please note that some details like version numbers may differ a bit in your session, that’s not important. From now on`iex`sessions will be stripped down to focus on the code. To exit`iex`press`Ctrl+C`twice.

It seems we are ready to go! We will use the interactive shell quite a lot in the next chapters to get a bit more familiar with the language constructs and basic types, starting in the next chapter.

> Note: if you are on Windows, you can also try`iex.bat --werl`which may provide a better experience depending on which console you are using.

## Running scripts {#running-scripts}

After getting familiar with the basics of the language you may want to try writing simple programs. This can be accomplished by putting the following Elixir code into a file:

```
IO
.
puts
"
Hello world from Elixir"
```

Save it as`simple.exs`and execute it with`elixir`:

```
$ 
elixir simple.exs
Hello world from Elixir
```

Later on we will learn how to compile Elixir code \(in[Chapter 8](http://elixir-lang.org/getting-started/modules-and-functions.html)\) and how to use the Mix build tool \(in the[Mix & OTP guide](http://elixir-lang.org/getting-started/mix-otp/introduction-to-mix.html)\). For now, let’s move on to[Chapter 2](http://elixir-lang.org/getting-started/basic-types.html).

## Asking questions {#asking-questions}

When going through this getting started guide, it is common to have questions, after all, that is part of the learning process! There are many places you could ask them to learn more about Elixir:

* [\#elixir-lang on freenode IRC](irc://irc.freenode.net/elixir-lang)
* [Elixir on Slack](https://elixir-slackin.herokuapp.com/)
* [Elixir Forum](http://elixirforum.com/)
* [elixir tag on StackOverflow](https://stackoverflow.com/questions/tagged/elixir)

When asking questions, remember these two tips:

* Instead of asking “how to do X in Elixir”, ask “how to solve Y in Elixir”. In other words, don’t ask how to implement a particular solution, instead describe the problem at hand. Stating the problem gives more context and less bias for a correct answer.

* In case things are not working as expected, please include as much information as you can in your report, for example: your Elixir version, the code snippet and the error message alongside the error stacktrace. Use sites like[Gist](https://gist.github.com/)to paste this information.



