# Guide

## The Free Lunch Is Over

- [x] http://www.gotw.ca/publications/concurrency-ddj.htm
- [x] https://en.wikipedia.org/wiki/Herb_Sutter
- [x] https://www.slideshare.net/Muhammad_Rizwan/the-free-lunch-is-over-43055538
- [x] https://softwareengineering.stackexchange.com/questions/212916/is-the-free-lunch-over

## The Actor Model

- [x] https://en.wikipedia.org/wiki/Actor_model
- [x] https://en.wikipedia.org/wiki/Carl_Hewitt
- [x] https://hal.archives-ouvertes.fr/hal-01163534v7/document
- [x] https://www.youtube.com/watch?time_continue=46&v=7erJ1DV_Tlo
- [x] https://www.brianstorti.com/the-actor-model/

## Erlang

> Erlang, foi desenvolvida pela Ericson em 1986, o objetivo era resolver o problema de telefonia da época. Possui uma VM chamada BEAM que é extratamente poderosa. Ela foi construida para garantir uma disponibilidade de 99,9999999%. O nome Erlang faz uma referência a "Ericsson Language".

> Joe Armstrong remarked in an interview with Rackspace in 2013: “If Java is 'write once, run anywhere', then Erlang is 'write once, run forever'.”[14]

> The Erlang view of the world, as Joe Armstrong, co-inventor of Erlang, summarized in his PhD thesis:

* Everything is a process.
* Processes are strongly isolated.
* Process creation and destruction is a lightweight operation.
* Message passing is the only way for processes to interact.
* Processes have unique names.
* If you know the name of a process you can send it a message.
* Processes share no resources.
* Error handling is non-local.
* Processes do what they are supposed to do or fail.

- [x] https://en.wikipedia.org/wiki/Erlang_(programming_language)

## Elixir/Processs (Actor Model)

- [x] http://eddwardo.github.io/elixir/2015/10/22/elixir-pingpong-table/
- [x] https://elixir-lang.org/getting-started/processes.html#spawn
- [x] https://eddwardo.github.io/elixir/2015/10/22/elixir-pingpong-table/
- [x] https://medium.com/elixirlabs/visualisation-of-elixir-supervision-tree-strategies-4d4cb8123138
- [x] https://medium.com/elixirlabs/anatomy-of-an-elixir-process-878030c37166
- [x] https://elixirschool.com/en/lessons/advanced/concurrency/
- [x] http://www.akitaonrails.com/2015/11/22/observing-processes-in-elixir-the-little-elixir-otp-guidebook
- [x] https://www.tutorialspoint.com/elixir/elixir_processes.htm
- [x] http://www.culttt.com/2016/07/11/working-processes-elixir/
- [x] https://cdn-images-1.medium.com/max/1600/1*9C_glQ0Nf4WIJKsfpnuiYA.png

## Elixir/Functional Programming

- [x] Concorrência (e Elixir): o que isso muda pra você? por George Guimarães - Rupy Campinas 2016 https://www.youtube.com/watch?v=MeCfWtMSWTE (55m:00)

#### Existe vida além do OO por Renan Ranelli - DevInSantos 2015

- [x] https://www.youtube.com/watch?v=njAMVB02Ag0 (52m:12s)

#### The Elixir of Life por Fabio Akita - DevInSantos 2015

- [x] https://www.youtube.com/watch?v=8Ng6TfAj7Sk (1h:00m)

#### Guru-SP 39: Do Ruby para o Elixir. E agora? por Renan Ranelli

- [x] https://www.youtube.com/watch?v=dQPGk6h59zs (58m:46s)

#### Elixir - FP (

- [x] https://www.youtube.com/watch?v=dqg1lgYERHY (23m:54s)
- [x] https://www.youtube.com/watch?v=7eYA8c8yABU (3h:39m)





- Não tem side effect

## Ref

- https://www.youtube.com/watch?v=GxnbUqPwuKw&t=9s
- https://medium.com/@kenmazaika/why-im-betting-on-elixir-7c8f847b58
- https://becoming-functional.com/a-brief-history-of-programming-c13d87b79337

# Elixir

## Tópicos

- http://images.slideplayer.com/9/2498272/slides/slide_5.jpg

- É uma linguagem Brasileira. :)

- Elixir é uma linguagem dinâmica e functional contruida para contruir aplicações escaláveis e manuteníveis.

- Funcional (dados imutáveis)(isso facilita a concorrência pois ela é tolerante a falhas)(pois não existe quebras nos dados)

- Concorrência nativa (processs)(são como thredes menores que se comunicam por mensagem dentro da BEAN)(cada processo não compartilha recursos) 

- Tolerante a falhas (Supervisors)(caso aconteça uma falha em um processo o Supervisores garantem que aquele processo isolado irá ser reiniciado)

- Foi desenvolvida pelo brasileiro José Valim, ele é um dos membros do rails core team e co-founder da plataformatec.

- Em 2010 Valim teve um problema de saúde LER (leção por esforço repetitivo). Então nessa época ele resolveu se dedicar a estudos, já que ele não poderia ficar programando tanto. Pra isso ele resolveu ler o livro Seven Languages in Seven Weeks, no livro tinha as linguages: Ruby, IO, Prolog, Scala, Erlang, Clojure, Haskell.. o que mais chamou anteção dele foi o Elarng. 

- Valim percebeu que os novos desenvolvedores não iram gostar muito da sintaxe do Erlang então decidiu dar uma roupagem nova criando o Elixir trazendo boas ideias do Ruby, Python, C#.. trouxe uma roupagem moderna para o Erlang

- Então em Janeiro de 2011 tivemos o primeiro commit do Elixir (https://github.com/elixir-lang/elixir/commit/337c3f2d569a42ebd5fcab6fef18c5e012f9be5b)

- Em Janeiro de 2012 ele fez uma proposta pra Plataformatec sobre se dedicar mais ao elixir 

- Em Maio de 2012 tivemos a primeira versão estavel 0.5

- Atualmente estamos na versão 1.6

- Elixir trouxe mais poder para o Erlang, pois trouxe um conjuto de ferramentas para o desenvolvedor ficar mais produtivo:

-- Mix 

```bash
mix deps              # Lists dependencies and their status
mix deps.clean        # Deletes the given dependencies' files
mix deps.compile      # Compiles dependencies
mix deps.get          # Gets all out of date dependencies
mix deps.unlock       # Unlocks the given dependencies
mix deps.update       # Updates the given dependencies
mix do                # Executes the tasks separated by comma
mix help              # Prints help information for tasks
mix local             # Lists local tasks
mix local.public_keys # Manages public keys
mix local.rebar       # Installs rebar locally
mix new               # Creates a new Elixir project
mix phoenix.new       # Create a new Phoenix v0.13.1 application
mix profile.fprof     # Profiles the given file or expression with fprof
mix run               # Runs the given file or expression
mix test              # Runs a project's tests
iex -S mix            # Starts IEx and run the default task
```

-- Hex (package manager)(212MI downloads)
-- Iex (Interpretador)

- Quem ta usando? https://elixir-companies.com/
- Comunidades: 

  - http://elixir-slackin.herokuapp.com/
  - https://www.meetup.com/elug_sp/
  - http://plataformatec.com.br/elixir-radar

- Elixir por defaul já trabalha com o conceito de microserver, pois ele já trabalha com o modelo The Actor Model

### Desvantagens

- Muitas libs você vai ter que fazer na mão
- CPU Intensive: Se você tiver que fazer uma app que tenha muito calculo número não é legal.
- Ecosistema pequeno
- Mudança de paradgma

## Ref

- [x] https://www.youtube.com/watch?v=dqg1lgYERHY **(23m:54s)**
- [x] https://www.youtube.com/watch?v=7eYA8c8yABU **(3h:39m)**
- [x] https://www.youtube.com/watch?v=MeCfWtMSWTE **(55m:00)**
- [x] https://www.youtube.com/watch?v=8Ng6TfAj7Sk **(1h:00m)**
- [x] https://www.youtube.com/watch?v=njAMVB02Ag0 **(52m:12s)**
- [x] https://www.youtube.com/watch?v=dQPGk6h59zs **(58m:46s)**
- [x] https://elixir-lang.org/getting-started/processes.html#spawn
- [x] https://eddwardo.github.io/elixir/2015/10/22/elixir-pingpong-table/




- https://github.com/benjamintanweihao/the-little-elixir-otp-guidebook-code/tree/master/chapter_1
- https://elixir-examples.github.io/
- https://elixirschool.com/en/
- https://trydis.github.io/2016/03/07/elixir-string-calculator/
- https://github.com/h4cc/awesome-elixir
- http://cloudless.studio/articles/17-elixir-vs-ruby-naming-conventions
- https://elixirforum.com/
- https://elixir-lang.org/getting-started/mix-otp/introduction-to-mix.html
- https://cfenollosa.com/blog/the-elixir-of-concurrency.html
- https://www.monterail.com/blog/2016/elixirconf-2016
- https://www.amberbit.com/blog/2016/2/24/how-elixirs-ecto-differs-from-rubys-activerecord/
- https://blog.portatext.com/2016/03/03/why-we-choose-elixir-to-power-our-sms-infrastructure/?utm_content=buffer93ad0&utm_medium=social&utm_source=twitter.com&utm_campaign=buffer
- http://blog.noredink.com/post/142689001488/the-most-object-oriented-language
- https://joearms.github.io/published/2016-03-13-Managing-two-million-webservers.html
- http://blog.plataformatec.com.br/2016/05/beyond-functional-programming-with-elixir-and-erlang/
- https://www.netguru.co/blog/10-companies-use-elixir
- https://www.youtube.com/watch?v=aA-XHI-EYcM
- https://elixir-lang.slack.com/messages/C0JUHGEMB/
- https://hex.pm/
- https://hexdocs.pm/iex/IEx.html
- https://www.meetup.com/elug_sp/members/
- https://gist.github.com/agustif/2f573557e5d2e4b42ed3b6cc4d285a8b
- https://www.youtube.com/watch?v=GxnbUqPwuKw
- https://www.youtube.com/watch?v=j_QWqs5gL3E&t=78s
- http://learningelixir.joekain.com/elixir-arc-with-a-single-module/
- http://blog.songsaboutsnow.com/elixir/processes/2016/04/06/intro-to-elixir-processes.html
- http://www.quentinthomas.com/automated-solutions-blog/2016/3/8/91n5rjioq4u9e6t88hpwlmiomolaqr
- http://blog.noredink.com/post/141444822213/pubsub-in-30-lines-of-elixir
- https://www.amberbit.com/blog/2016/5/10/creating-elixir-libraries-as-otp-applications/
- http://crypt.codemancers.com/posts/2016-01-24-understanding-exit-signals-in-erlang-slash-elixir/
- https://rockyj.in/2016/06/19/elixir_pi_calc.html
- http://tech.strofcon.org/2016/04/lets-build-something-elixir-part-3.html
- http://tech.strofcon.org/2016/04/lets-build-something-elixir-part-4.html
- http://blog.plataformatec.com.br/2016/04/debugging-techniques-in-elixir-lang/?utm_content=buffer16787&utm_medium=social&utm_source=twitter.com&utm_campaign=buffer
- http://blog.plataformatec.com.br/2016/04/how-to-trace-elixir-nodes-with-erlyberly/
- http://plataformatec.com.br/elixir-radar/
- http://plataformatec.com.br/elixir-radar/weekly-newsletter
- https://orestis.gr/functional-puzzles-part-1/?utm_campaign=elixir_radar_132&utm_medium=email&utm_source=RD+Station
- https://medium.com/@DFilipeS/how-i-rented-a-nice-place-to-live-using-elixir-and-a-facebook-messenger-chat-bot-836f79498c5c
- https://m.alphasights.com/simple-web-servers-with-plug-and-cowboy-34f7a174f252
- http://ezgr.net/increasing-security-erlang-ssl-cowboy/
- http://www.automatingthefuture.com/blog/2016/3/21/ai-generate-and-test-elixir
- http://learningelixir.joekain.com/mix-profile/
- https://keathley.io/2016/04/09/elixir-guard-clauses.html
- https://yos.io/2016/03/26/type-checking-in-elixir/
- https://trydis.github.io/2016/03/07/elixir-string-calculator/
- https://www.youtube.com/watch?v=YSQmIciT0xE
- http://elviovicosa.com/blog/2016/07/13/deploying-elixir-releases.html
- https://github.com/elixir-lang/elixir/commit/337c3f2d569a42ebd5fcab6fef18c5e012f9be5b
- https://elixir.career
- https://rdstation-static.s3.amazonaws.com/cms%2Ffiles%2F7452%2F1518712802Three_Adoption_Stories_of_Adopting_Elixir.pdf?utm_campaign=auto-response_-_chapter_three_adoption_stories&utm_medium=email&utm_source=RD+Station
- https://subvisual.co/blog/posts/137-tutorial-deploying-elixir-applications-with-docker-and-digital-ocean/
- https://orestis.gr/live-debugging-an-elixir-memory-process-leak/
- http://www.anilwadghule.com/2016/09/10/ruby-concurrency-compared.html
- http://trivelop.de/2018/03/26/flow-elixir-using-plug-like-token/
- http://milhouseonsoftware.com/2016/05/08/measuring-your-elixir-application/
- https://www.brianstorti.com/process-registry-in-elixir/
- https://www.brianstorti.com/getting-started-with-plug-elixir/

# Phoenix

## Tópicos

-

## Ref

- https://hackernoon.com/a-free-introduction-to-elixir-otp-ecto-and-phoenix-228d0e994fc1
- https://medium.brianemory.com/elixir-phoenix-creating-an-app-part-6-using-the-youtube-api-5ff58082088e
- https://medium.com/@fredjourney/how-to-build-a-phoenix-hello-world-rest-api-5fc9e3acf331
- https://medium.com/@brucepomeroy/create-an-elixir-umbrella-project-containing-a-phoenix-app-and-build-a-release-with-distillery-46371f2617df
- https://medium.com/everydayhero-engineering/create-an-elixir-phoenix-api-part-1-initial-barebones-setup-7c840a6c4c5c
- https://sergiotapia.me/how-to-version-your-phoenix-framework-api-10e86e866577
- http://elviovicosa.com/blog/2016/07/22/phoenix-api-versioning-url.html
- https://blog.codeship.com/an-introduction-to-apis-with-phoenix/
- https://becoming-functional.com/building-a-rest-api-with-phoenix-and-elixir-b12dcec302c5
- https://becoming-functional.com/a-phoenix-and-elixir-rest-api-part-2-dc00e8b73c9d
- https://elixircasts.io/versioned-api-with-phoenix
- https://renatomoya.github.io/2015/05/09/Building-a-versioned-REST-API-with-Phoenix-Framework.html
- http://work.stevegrossi.com/2016/07/11/building-a-chat-app-with-elixir-and-phoenix-presence/
- https://sergiotapia.me/killing-all-socket-connections-for-a-user-in-phoenix-framework-915148e98186
- https://medium.com/@ejpcmac/persistent-logins-in-elixir-with-expected-70b9aac2bcae
- https://dockyard.com/blog/2018/02/12/what-s-new-in-phoenix-development-february-2018?utm_campaign=elixir_radar_131&utm_medium=email&utm_source=RD+Station
- https://dockyard.com/blog/2018/02/12/what-s-new-in-phoenix-development-february-2018?utm_campaign=elixir_radar_131&utm_medium=email&utm_source=RD+Station
- https://niallburkley.com/blog/changing-primary-keys-in-ecto/?utm_campaign=elixir_radar_131&utm_medium=email&utm_source=RD+Station
- https://joaquimadraz.com/guide-to-deploy-an-elixir-phoenix-app-to-aws-ecs?utm_campaign=elixir_radar_132&utm_medium=email&utm_source=RD+Station
- https://pspdfkit.com/blog/2018/how-to-run-your-phoenix-application-with-docker/?utm_campaign=elixir_radar_132&utm_medium=email&utm_source=RD+Station
- http://devonestes.herokuapp.com/whats-the-deal-with-module-attributes?utm_campaign=elixir_radar_132&utm_medium=email&utm_source=RD+Station
- https://tokafish.com/rails-to-phoenix-querying-with-ecto/
- https://blog.fourk.io/rails-cli-commands-for-elixir-phoenix-88cb7da45fe7
- https://hackernoon.com/a-free-introduction-to-elixir-otp-ecto-and-phoenix-228d0e994fc1
- https://medium.com/@miguel.coba/building-a-game-with-phoenix-channels-a3e6b390cfcc
- https://joaquimadraz.com/guide-to-deploy-an-elixir-phoenix-app-to-aws-ecs
- https://hackernoon.com/phoenix-application-deployment-with-nanobox-1d2274f061e5
- https://medium.com/@mschae/measuring-your-phoenix-app-d63a77b13bda
