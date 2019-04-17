dlist - реализация двухсвязных списков на Common Lisp
=================================================================
dlist - это библиотека Common Lisp, которая реализует структуру двусвязного списка data.  
dlist предоставляя множество операций над двусвязными списками, или dlists, которые описаны в файле documents.html, 
который доступен вместе с источником.  
Если ваша реализация lisp поддерживает [расширяемые пользователем последовательности][1]  
(в настоящее время только SBCL и ABCL выполняют), вы сможете использовать стандартные функции Common Lisp sequence (map, lower, и т.д.) со списками.  
У dlist нет никаких зависимостей, кроме обычной реализации lisp.  

dlist is a Common Lisp library that implements the doubly-linked list
data structure. dlist provides many operations on doubly-linked lists,
or dlists, which are documented in the file documentation.html , which
is available with the source. If your lisp implementation supports
[user-extensible sequences][1] (which only SBCL and ABCL do
currently), you will be able to use the standard Common Lisp sequence
functions (map, reduce, etc.) with dlists. dlist does not have any
dependencies other than a common lisp implementation.

О данном коде
---------------
Данный код - это форк оригинальной библиотеки dlist ([http://github.com/krzysz00/dlist](GitHub)). Оригинальная библиотека доступна через Quicklisp. Недостатком оригинала является явный дефицит функций, например, нельзя удалить элемент из середины или вставить его в середину списка. Форк зависит от [https://bitbucket.org/budden/budden-tools](budden-tools), которая тоже недоступна через quicklisp (во всяком случае, я ничего не делал для её доступности).

Частичная русификация
----------------------
Новый код и документация частично русифицированы. 

Obtaining and installing dlist
------------------------------
Получение и установка dlist
---------------------------
Всё как обычно для библиотек не под quicklisp. Use:

    (asdf:oos 'asdf:test-op :dlist)

to run the test suite.

dlist is licensed under the 3-Clause BSD Licence, see the file COPYING
for details.

Contact Information
-------------------
Пишите на github. 

Что надо исправить
-------------------
Изменить название. Больше тестов. 

[1]: http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.65.1604&rep=rep1&type=pdf
