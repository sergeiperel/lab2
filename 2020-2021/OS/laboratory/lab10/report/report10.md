---
# Front matter
lang: ru-RU
title: "Отчёт по лабораторной работе № 10"
author: "Перелыгин Сергей Викторович"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором Emacs.

# Выполнение лабораторной работы

1. Откроем редактор Emacs с помощью команды «emacs &».

![Рдактор emacs](images/1.png){ #fig:001 width=70% }

![Рдактор emacs](images/2.png){ #fig:002 width=70% }

2. Создадим файл lab07.sh с помощью комбинации «Ctrl-x» «Ctrl-f». 

![Создание файла lab07.sh](images/3.png){ #fig:002 width=70% }

3. В открывшемся буфере наберем необходимый текст. 

![Набираем текст](images/4.png){ #fig:004 width=70% }

4. Сохраним файл с помощью комбинации «Ctrl-x»«Ctrl-s».

5. 
1) Вырежем одной командой целую строку («Сtrl-k»).

![Вырезаем строку](images/5.png){ #fig:004 width=70% }

2) Вставим эту строку в конец файла («Ctrl-y»). 

![Вставляем строку в конец файла](images/6.png){ #fig:006 width=70% }

3) Выделим область текста («Ctrl-space»).

![Выделяем область текста](images/6.png){ #fig:007 width=70% }

4) Скопируем область в буфер обмена («Alt-w»).

5) Вставим область в конец файла («Ctrl-y»).
 
![Вставляем текст в конец файла](images/7.png){ #fig:007 width=70% }

6) Вновь выделим эту область(«Ctrl-space») и на этот раз вырежем её («Ctrl-w»).

![Выделяем эту область](images/8.png){ #fig:008 width=70% }

![Вырезаем эту область](images/9.png){ #fig:009 width=70% }
 
 
7) Отменим последнее действие («Ctrl-/»).
   
![Отменяем последнее действие](images/10.png){ #fig:010 width=70% } 
   
6. 
1) Переместим курсор в начало строки («Ctrl-a»).

2) Переместим курсор в конец строки («Ctrl-e»).

3) Переместим курсор в начало буфера («М-<») .

4) Переместим курсор в конец буфера («М->»).

7. 
1) Выведем список  активных  буферов  на  экран  («Ctrl-x»«Ctrl-b»). 

![Список активных буферов](images/12.png){ #fig:011 width=70% } 

2) Переместимся во вновь открытое окно («Ctrl-x o») со  списком открытых буферов и переключимся на другой буфер (для этого необходимо нажать на «enter» после выбора необходимого буфера).

![Переключаемся во вновь открытое окно](images/13.png){ #fig:012 width=70% } 

3) Закроем это окно («Ctrl-x 0»).

![Закрываем окно](images/14.png){ #fig:013 width=70% } 

4) Теперь вновь переключимся между буферами, но уже без вывода их списка на экран («Ctrl-x b»).

![Переключаемся между буферами](images/15.png){ #fig:014 width=70% } 

![Переключаемся между буферами](images/16.png){ #fig:015 width=70% } 

![Переключаемся между буферами](images/17.png){ #fig:016 width=70% }

8. 
1) Поделим фрейм  на  4  части:  разделим  фрейм  на  два  окна  по вертикали («Ctrl-x 3»), а затем каждое из этих окон на две части по горизонтали («Ctrl-x 2»).

![Поделим фрейм на 4 части](images/18.png){ #fig:017 width=70% }

2) В каждом из четырёх созданных окон откроем новый буфер (файл) и введем несколько строк текста. Для этого предварительно создадим эти файлы с помощью команд «touch file1.txt»,«touch file2.txt», «touch file3.txt», «touch file4.txt».

![Создаем файлы](images/19.png){ #fig:018 width=70% }

![Печатаем текст](images/20.png){ #fig:019 width=70% }

9. 
1) Переключимся в режим поиска («Ctrl-s») и найдем несколько слов, присутствующих в тексте.

![Ищем слово Emacs](images/21.png){ #fig:020 width=70% }

2) Переключимся между  результатами  поиска,  нажимая «Ctrl-s».

3) Выйдем из режима поиска, нажав «Ctrl-g».

![Выходим из режима поиска](images/22.png){ #fig:021 width=70% }

4) Перейдем в  режим  поиска  и  замены  («М-%»),  введем текст, который следует найти и заменить, нажмем «enter», затем введем текст для  замены.  После  того  как  будут  подсвечены  результаты  поиска, нажмем «!» для подтверждения замены.

![Заменяем слово в тексте](images/23.png){ #fig:022 width=70% }

![Заменяем слово в тексте](images/24.png){ #fig:023 width=70% }

![Заменяем слово в тексте](images/25.png){ #fig:024 width=70% }

![Заменяем слово в тексте](images/26.png){ #fig:025 width=70% }

5) Пробуемдругой режим поиска, нажав «M-s o»

![Заменяем слово в тексте](images/27.png){ #fig:026 width=70% }

# Ответы на контрольные вопросы

1. Emacs - один  из  наиболее  мощных  и  широко  распространённых редакторов,  используемых  в  мире Unix.  По  популярности  он соперничает с редактором vi и его клонами. В зависимости от ситуации, Emacs может быть:

- текстовым редактором;

- программой для чтения почты и новостей Usenet;

- интегрированной средой разработки (IDE);

- операционной системой и т.д.

Всё  это  разнообразие  достигается  благодаря  архитектуре Emacs, которая  позволяет  расширять  возможности  редактора  при  помощи языка Emacs  Lisp. На  языке C написаны  лишь  самые  базовые  и низкоуровневые  части Emacs, включая  полнофункциональный интерпретатор языка Lisp. Таким образом, Emacs имеет встроенный язык программирования, который может использоваться для настройки, расширения  и  изменения  поведения  редактора.  В  действительности, большая часть того редактора, с которым пользователи Emacs работают в наши дни,написана на языке Lisp.

2. Основную трудность для новичков при освоенииданного редактора могутсоставлять  большое  количество  команд,  комбинаций  клавиш, которые не получится все запомнить с первого раза и поэтому придется часто обращаться к справочным материалам.

3. Буфер –это  объект,  представляющий  собой  текст. Если  имеется несколько буферов, то редактировать можно только один. Обычно буфер считывает данные из файла или записывает в файл данные из буфера.Окно –это область экрана, отображающая буфер. При запуске редактора отображается одно окно, но при обращении к некоторым функциям могут открыться дополнительные окна. Окна Emacs и окна графической среды XWindow–разные вещи. Одно окно XWindow может быть разбито  на  несколько  окон  в  смысле Emacs,  в  каждом  из  которых отображается отдельный буфер.

4. Да, можно.

5. При запуске Emacs по умолчанию создаются следующие буферы:

- «scratch»(буфер для несохраненного текста)

- «Messages»(журнал ошибок, включающий также информацию, которая появляется в области EchoArea)

- «GNUEmacs»(справочный буфер о редакторе)

6. C-c |сначала, удерживая «ctrl»,нажимаю «c»,после –отпускаю обе клавишии нажимаю «|»
 C-cC-|сначала, удерживая «ctrl»,нажимаю «с», после –отпускаю обе клавиши и, удерживая «ctrl», нажимаю «|»
 
7. Чтобы  поделить  окно  на  две  части  необходимо  воспользоваться комбинацией «Ctrl-x 3»(по вертикали) или «Ctrl-x 2» (по горизонтали).

8. Настройки Emacs сохранятся в файле .emacs.

9. По  умолчанию  клавиша «←» удаляет  символ перед  курсором, нов редакторе  её  можно  переназначить.  Для  этого  необхдимоизменить конфигурацию файла .emacs.

10. Более удобным я считаю редактор emacs, потому что в нем проще открывать другие файлы, можно использовать сразу несколько окон, нет «Командного режима», «Режима ввода», «Режима командной строки», которые  являются  немного  непривычными  и  в  какой-то  степени неудобным

# Выводы

в ходе выполнения данной лабораторной работы я познакомился с операционной системой Linux и получил практические навыки работы с редактором Emacs.







