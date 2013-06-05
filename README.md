# Play + Checkstyle + PMD #

## Background ##

This repo attempts to answer the [StackOverflow question](http://stackoverflow.com/questions/16929442/how-to-integrate-checkstyle-and-pmd-into-play-framework-build-scala-file) "How to integrate checkstyle and PMD into Play framework Build.scala file".

This repo will not be maintained separately from the [sbt-code-quality](https://github.com/ymasory/sbt-code-quality.g8) giter8 template that shows how to use Checkstyle & PMD in a vanilla Scala app.


## Run ##

```
$ cd play-pmd-checkstyle
$ play
[info] Loading project definition from /Users/yuvi/Desktop/play-pmd-checkstyle/project
[info] Set current project to quality (in build file:/Users/yuvi/Desktop/play-pmd-checkstyle/)
       _            _
 _ __ | | __ _ _  _| |
| '_ \| |/ _' | || |_|
|  __/|_|\____|\__ (_)
|_|            |__/

play! 2.1.1 (using Java 1.7.0_21 and Scala 2.10.0), http://www.playframework.org

> Type "help play" or "license" for more information.
> Type "exit" or use Ctrl+D to leave this console.

[quality] $ checkstyle
[info] using checkstyle args List(-c, /Users/yuvi/Desktop/play-pmd-checkstyle/project/checkstyle-config.xml, -f, xml, -r, /Users/yuvi/Desktop/play-pmd-checkstyle/app, -o, /Users/yuvi/Desktop/play-pmd-checkstyle/target/checkstyle-report.xml)
[success] Total time: 1 s, completed Jun 5, 2013 1:51:58 PM
[quality] $ pmd
[info] using pmd args List(/Users/yuvi/Desktop/play-pmd-checkstyle/app, html, /Users/yuvi/Desktop/play-pmd-checkstyle/project/pmd-ruleset.xml, -reportfile, /Users/yuvi/Desktop/play-pmd-checkstyle/target/pmd-report.html)
[success] Total time: 1 s, completed Jun 5, 2013 1:52:00 PM
[quality] $
```
