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

เมื่อลง Elixir เสร็จแล้ว เราจะพบว่ามีคำสั่งใหม่ขึ้นมา 3 อันคือ iex, elixir, และ elixirc ถ้าคุณคอมไพล์ Elixir จากซอร์สโค้ด จะพบไฟล์ที่ถูกคอมไพล์แล้ว อยู่ในภายใต้ไดเรกทอรี่ bin

สำหรับตอนนี้, เริ่มต้นโดยพิมพ์คำสั่ง iex \( หรือ iex.bat สำหรับคนที่ใช้วินโดว์\) เพื่อเข้าใช้ Interactive Elixir \( คล้ายๆกับการใช้ python shell \), เราสามารถที่จะพิมพ์โปรแกรมหรือคำสั่งของ Elixir แล้วได้ผลลัพธ์ได้เลยทันที ซึ่งทำให้เราสามารถเรียนภาษา Elixir จากช่องทางนี้ได้เช่นกัน

เปิด iex แล้วลองพิมพ์ข้อความ เหล่านี้ลงไป \(พิมพ์หลังเครื่องหมาย &gt;  เช่น &gt; 40 + 2  คือพิมพ์ 40 + 2 แล้วกด Enter \)

```ruby
Erlang/OTP 19 [erts-8.1] [source] [64-bit] [smp:4:4] [async-threads:10] [hipe] [kernel-poll:false] [dtrace]

Interactive Elixir (1.4.0) - press Ctrl+C to exit (type h() ENTER for help)
iex(1)>  40 + 2
42
iex(2)> "hello" <
> " world"
"hello world"
```

ตรงเลขเวอร์ชั่น อาจจะแตกต่างกัน แต่ไม่มีความสำคัญอะไรนะคับ ตอนนี้ เราเน้นที่การเขียนโปรแกรมก่อน และวิธีการออกจาก Interactive Shell ทำได้โดยการพิมพ์ Ctrl + C สองครั้ง

ตอนนี้ เราพร้อมกันแล้ว และในบทถัดๆไปเราจะใช้ interactive shell กันเยอะขึ้นมากในการเขียนโปรแกรมเริ่มต้น

> บันทึก: ถ้าคุณใช้ Windows แนะนำให้พิมพ์คำสั่ง iex.bat --werl จะดีกว่าการใช้ iex.bat อย่างเดียว

## Running scripts {#running-scripts}

เรามาลองสร้างโปรแกรมง่ายๆสักอัน โดยพิมพ์ข้อความเหล่านี้ลงในไฟล์

```ruby
IO.puts "Hello world from Elixir"
```

แล้วบันทึกไฟล์ในชื่อ simple.exs แล้วรันโดยใช้คำสั่ง elixir :

```ruby
$ elixir simple.exs
Hello world from Elixir
```

หลังจากนี้ เราจะได้เรียนรู้วิธีการคอมไพล์โปรแกรม Elixir \(ใน  [บทที่ 8](http://elixir-lang.org/getting-started/modules-and-functions.html)\) และการใช้คำสั่ง Mix \(ในบท[ Mix & OTP Guide](http://elixir-lang.org/getting-started/mix-otp/introduction-to-mix.html)\) อีกครั้ง สำหรับตอนนี้ ไปเรียนจาก [บทที่ 2 ](http://elixir-lang.org/getting-started/basic-types.html)ก่อนดีกว่า

## Asking questions {#asking-questions}

When going through this getting started guide, it is common to have questions, after all, that is part of the learning process! There are many places you could ask them to learn more about Elixir:

* [\#elixir-lang on freenode IRC](irc://irc.freenode.net/elixir-lang)
* [Elixir on Slack](https://elixir-slackin.herokuapp.com/)
* [Elixir Forum](http://elixirforum.com/)
* [elixir tag on StackOverflow](https://stackoverflow.com/questions/tagged/elixir)

When asking questions, remember these two tips:

* Instead of asking “how to do X in Elixir”, ask “how to solve Y in Elixir”. In other words, don’t ask how to implement a particular solution, instead describe the problem at hand. Stating the problem gives more context and less bias for a correct answer.

* In case things are not working as expected, please include as much information as you can in your report, for example: your Elixir version, the code snippet and the error message alongside the error stacktrace. Use sites like[Gist](https://gist.github.com/)to paste this information.



