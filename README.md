# bookmarks_erlnag-elixir
Erlang/Elixir 関係の記事のブックマーク


# Erlang
## 設計思想や基本構造など
- [The Zen of Erlang](http://ferd.ca/the-zen-of-erlang.html) Erlang の基本的な考えなどを説明
- [Erlang Garbage Collection Details and Why It Matters](https://hamidreza-s.github.io/erlang%20garbage%20collection%20memory%20layout%20soft%20realtime/2015/08/24/erlang-garbage-collection-details-and-why-it-matters.html) Erlang の GC, Erlang の OS プロセスで共通の shared heap とかの説明
- [How do Erlang Microprocesses work internally?](https://www.reddit.com/r/erlang/comments/4sogzb/how_do_erlang_microprocesses_work_internally/) プロセスのスケジューリングなど内部的な動作に関するスレッド
- [Welcome to BEAM VM Wisdoms!](http://beam-wisdoms.clau.se/en/latest/) BEAMの内部構造などの簡単な説明

## Cowboy/Ranch
- [Erlang/OTP architectures: cowboy](https://medium.com/@kansi/erlang-otp-architectures-cowboy-7e5e011a7c4f#.wu3l885ab) Cowboyというよりは Ranch の簡単な説明



# Elixir
## 設計思想や基本構造など
- [Erlang(Elixir)の使いどころについて使ってる人から教わった話](http://togetter.com/li/977171) Beam の特性など

## プロセス管理
- [Foreign Processes and Phoenix](https://shift.infinite.red/foreign-processes-and-phoenix-555179c24151#.tzw8s1uk1) Ports と Supervisors による外部プロセスの稼働監視

## Ecto
- [Understanding Elixir’s Ecto Querying DSL: The Basic] (https://www.sitepoint.com/understanding-elixirs-ecto-querying-dsl-the-basics/) Ecto query の基本
  - [Elixir’s Ecto Querying DSL: Beyond the Basic](https://www.sitepoint.com/elixirs-ecto-querying-dsl-beyond-the-basics/) Ecto query の応用編
- [[翻訳] Ectoを使った組み立て可能なクエリ](http://qiita.com/HirofumiTamori/items/b71ca312778e42326017)

## Test/Debug
- [Debugging Phoenix with IEx.pry](https://medium.com/@diamondgfx/debugging-phoenix-with-iex-pry-5417256e1d11#.eyjvklsn7) Python の pdb.set_trace() みたいなことをやる方法
- [ExUnit Cheat Sheet](http://blog.lucidsimple.com/2016/01/31/exunit-cheat-sheet.html?utm_campaign=elixir_radar_39&utm_medium=email&utm_source=RD+Station) チートシート
- [Easy Mocking in Elixir with Meck](http://blog.lucidsimple.com/2016/01/04/easy-mocking-in-elixir-with-meck.html) Meck によるモックテストのやり方
- [Writing Acceptance tests in Phoenix](http://blog.plataformatec.com.br/2016/01/writing-acceptance-tests-in-phoenix/?utm_campaign=elixir_radar_34&utm_medium=email&utm_source=RD+Station) hound による acceptance test の例
- [Special Processes in OTP](http://blog.carbonfive.com/2016/06/28/special-processes-in-otp/) Erlang の :sys, :proc_lib の利用を通して :sys.statistics, :sys.trace の使い方を簡単に説明


## OTP
### GenServers
- [Let's talk about GenServers](http://codingwithaxe.com/lets-talk-about-genserver-in-elixir/) Elixir での GenServer の書き方の簡単な説明
- [Creating Elixir libraries as OTP applications](https://www.amberbit.com/blog/2016/5/10/creating-elixir-libraries-as-otp-applications/) 簡単な chat ボットを GenServer で作る

### Supervisor
- [Supervisorを使ってプロセス管理を行う](http://qiita.com/ak-ymst/items/c2efcee60dd774062429)

## Syntax
- [Elixir Quick Reference](https://github.com/itsgreggreg/elixir_quick_reference) Elixir の書式のリファレンス
- [Elixir Examples](https://elixir-examples.github.io/) アトムから文字列への変換方法など、簡単な tips 集
- [Elixir Best Practices - Deeply Nested Maps](https://dockyard.com/blog/2016/02/01/elixir-best-practices-deeply-nested-maps) 深い階層のMapやListをKernel.put_in/3で簡単に扱う方法の説明
- [@specでのintegerとString.tの違い](https://www.reddit.com/r/elixir/comments/4v2ss2/help_me_understand_types_in_documentation_specs/)

### Protocol
- [Extensible Design with Protocols](https://blog.drewolson.org/extensible-design-with-protocols/) protocol とその使い方の簡単な説明

## SMTP
- [Announcing Bamboo, Email with a Functional Twist](https://robots.thoughtbot.com/announcing-bamboo-email-with-a-functional-twist?utm_campaign=elixir_radar_46&utm_medium=email&utm_source=RD+Station) Bamboo によるメール送信の簡単な説明

## リリース
- [Distillery vs. Exrm vs. Relx](http://bitwalker.org/posts/2016-07-21-distillery-vs-exrm-vs-relx/) 次世代版 Exrm である Distillery について作者の考えがまとまっている

## ETS
- [Make Phoenix Even Faster with a GenServer-backed Key Value Store](https://robots.thoughtbot.com/make-phoenix-even-faster-with-a-genserver-backed-key-value-store) よくある、Supervisor 配下で ETS を使ってキャッシングする例だけどよくまとまってる。
