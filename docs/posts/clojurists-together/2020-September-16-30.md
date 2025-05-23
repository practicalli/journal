---
title: Practicalli Project Update 3
date: 2020-09-30
authors:
  - practicalli
categories:
  - clojurists-together
---

![Clojurists Together Logo](https://raw.githubusercontent.com/practicalli/graphic-design/live/buttons/practicalli-clojurists-together-button.svg){align=right loading=lazy style="height:150px;width:150px"}

Continuing the Live broadcasts covering the developmment of the Banking on Clojure web application.
- [084 - Banking On Clojure - Part5 - Generated database records from clojure.spec](https://youtu.be/Cn5QX9nL7jU)
- [085 - Banking On Clojure - Part6 - Refactor database schema, specs and namespaces](https://youtu.be/e4QInyWa1bM)

<!-- more -->

## Practicalli Clojure

New sections and Pages:
* [Coding Challenges section](http://practical.li/clojure/coding-challenges/)
* [Unit testing fixtures](http://practical.li/clojure/testing/unit-testing/fixtures/)

Added Code Challenges section, covering the Clojure challenges available in 4Clojure.com, Exercism.io, CodwWars.com, ClojureScript Koans and Advent of Code.

A quick guide to using each of the Code challenge websites was provided and tips to using them effectively.

GitHub code repositories for the Practicalli [4Clojure guides](https://github.com/practicalli/four-clojure/), [codewars-guides](https://github.com/practicalli/codewars-guides) and [exercism-guides](https://github.com/practicalli/exercism-clojure-guides) were included, along with the [4Clojure guides video playlist](https://www.youtube.com/playlist?list=PLpr9V-R8ZxiDB_KGrbliCsCUrmcBvdW16) which walks through the solution to over 60 challenges and different approaches to solving them.

Several 4Clojure and Exercism challenges have been added as solution walk-through, showing the design thinking behind the solution in the website.  More of these will be converted from the solution code repositories as time allows, along with a video showing the REPL driven development experience.

Added [Unit testing fixtures](http://practical.li/clojure/testing/unit-testing/fixtures/) page with examples from Banking on Clojure project.  Also mentioned test selectors as a way to organize slower fixtures.

Started creating project templates for use with clj-new, to create deps.edn projects useful for beginners and experienced developers alike.  A section on writing your own custom templates will be added to the Practicalli Clojure book in October.

Continuing to create scripts for video screencasts for a series on the Clojure CLI tools, covering the usage from the latest release (1.10.1.697). The series will convey the developer experience and common practices.

Continue testing Clojure CLI pre-release and enhancing the aliases in practicalli/clojure-cli-config, no issues found so far.


## Clojure WebApps

Redesign the database schema and clojure.spec specifications to simplify the use of generative testing with specifications and in general make the specifications easier to work with.

Using generative testing with the database.  Specifications are used to generate random data to test the database CRUD functions, validating the results of those functions against clojure specs.

Added code to create and delete the development database which is called from fixture functions within the handler-helper-test namepace.  The tests now run successfully via the CirceCI service.

Using kaocha profiles to configure different behavior in the development environment and when running on the CI server, specifically file change watcher and test output.


## Practicalli Spacemacs

Now Emacs 27 is the default, trying out Ligature support in Emacs.  Added the unicode layer with variables to include ligatures.  Initially switching to the Fira code font which contains a wide range of ligatures in the font already.

Will try the [Ligaturizer project](https://github.com/ToxicFrog/Ligaturizer) to add Fira Code ligatures to the Ubuntu Mono font, the preferred font used by Practicalli.
