# kotlin_slow_start
Котлин. Медленный старт

## Окружение

1. skdman
Идем на https://sdkman.io/ и скачиваем sdkman 
или с помощью bash

```bash
curl -s https://get.sdkman.io | bash
```

2. java \ jdk
Любым доступным способом ставим jdk версии 8.0.х или 9.0.х
Если windowds то скачиваем тут https://adoptopenjdk.net/releases.html?variant=openjdk8&jvmVariant=hotspot

или с помощью sdkman
```bash
 sdk install java 8.0.222.hs-adpt
```

3. gradle
Таск менеджер и он же пакетный менеджер
```
 sdk install gradle
 ```
 
 ## IDE
 
 Или Idea
 https://www.jetbrains.com/idea/download/
 
 Или Visual Code
 https://code.visualstudio.com/
 Если первый раз, то лучше idea, community version вполне хватит
 
 
 ## Hello world
 
 Создание проекта с помощью gradle самый удобный вариант
 ```bash
mkdir hello_world
cd ./hello_world
gradle init
```
выведет
```
Select type of project to generate:
  1: basic
  2: application
  3: library
  4: Gradle plugin
Enter selection (default: basic) [1..4] 2 
 ```
 где выбираем в данной ситуации 2 (application)
 
 
 ```
 Select implementation language:
  1: C++
  2: Groovy
  3: Java
  4: Kotlin
  5: Swift
```
А тут выбираем 4 (Kotlin)



```
Select build script DSL:
  1: Groovy
  2: Kotlin
```
А вот тут стоит подумать, я выбираю всегда 2 (Kotlin DSL), потому что 1. мне нравится как тут работает автокомплит, и 2. я знаю Kotlin в отличии от Groovy

ок. выбираем 2 (Kotlin)

Далее имя проекта оставляем как есть, просто жмем на клавиатуре enter и имя пакета опять enter.
Проверяем что все ок, выполняем
```bash
 ./gradlew run
 ```
Если будет 
```
$ ./gradlew run
Downloading https://services.gradle.org/distributions/gradle-5.6.2-bin.zip
.........................................................................................

> Task :run
Hello world.

```
То можно теперь открывать проект в IDE

## Введение
На текущий момент самый простой вариант это вот этот курс

https://www.programiz.com/kotlin-programming/hello-world

Если совсем ничего не получается, то всегда можно пойти в онлайн песочницу https://play.kotlinlang.org/ , но в ide конечно удобнее
