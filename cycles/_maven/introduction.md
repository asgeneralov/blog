---
title: Введение в maven
layout: default
sort: 1
---

# Введение в maven
Maven это утилита, которая относится к классу программ типа сборщик или менеджер пакетов. Подобные программы существуют для большинства популярных языков программирования, например: bundler в ruby, npm в NodeJs, NuGet в C# и так далее. Для языка Java существует целых 3 сборщика -- это Ant, Maven и Gradle (в порядке появления). 

В то время как Ant представляет собой скорее средство автоматизации повторяющихся задач, Maven вводит ряд концепций для управления зависимостями проекта и создания различных артефактов. Центральной единицей управления проектом является файл pom.xml (от Project Object Model). В этом файле описываются артефакты которые требуется собрать и зависимости проекта в формате Group:Artifact:Version. Этому формату зависимостей следует и Gradle, который будучи полностью соместимым с Maven, использует для управления проектом файл build.groovy на языке Groovy, а так же имеет ряд других особенностей связанных оптимизацией сборки проекта.

Не смотря на растущую популярность Gradle и слегка многословный формат POM в Maven (благодаря формату XML), Maven все еще остается стандартным выбором для большинства Java проектов. Это связано с тем, что за время свого существования Maven (создан в 2002, автор Jason van Zyl для фонда Apache Software Foundation), оброс многими нужными и полезным возможностями, которые помогают Java программистам создавать артефакты и решать проблемму &laquo;ада зависимостей&raquo; (от анг. dependency hell).