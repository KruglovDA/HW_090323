#	Заголовки
Язык разметки Markdown поддерживает 2 стиля обозначения заголовков: подчеркивание и выделение символом («#»).
Выделение заголовков с помощью подчеркивания производится знаками равенства («=») в случае, если заголовок первого уровня, и дефисами («-») в случае, если заголовок второго уровня. Количество знаков подчеркивания не ограничивается.
При выделении заголовков с помощью символа («#») используется от одного до шести данных символов, которые устанавливаются в начале строки (перед заголовком). В данном случае количество символов соответствует уровню заголовка. Кроме того, заголовок возможно снабдить закрывающимися символами («#»), хотя это и не является обязательным. Количество закрывающихся символов не обязано соответствовать количеству начальных символов. Уровень заголовка определяется по количеству начальных символов.  
Заголовки первого и второго уровней, выполненные с помощью подчеркивания, выглядят следующим образом:

    Заголовок первого уровня
    ========================
    Заголовок второго уровня
    -------------------------
Заголовки первого, третьего и шестого уровней, выполненные с помощью символа («#»), выглядят следующим образом:
	
    #  Заголовок первого уровня
    ### Заголовок третьего уровня
    ###### Заголовок шестого уровня
Приведенные выше заголовки, выполненные с помощью символа («#») тождественны следующим:

    #  Заголовок первого уровня #
    ### Заголовок третьего уровня ###
    ###### Заголовок шестого уровня ######
В результате на экран выводится следующее:    
Заголовок первого уровня
========================

Заголовок второго уровня
------------------------

#  Заголовок первого уровня
### Заголовок третьего уровня
###### Заголовок шестого уровня

##### <a name="Emphasis"></a> 	Выделение текста
Markdown воспринимает звёздочки «*» и символы подчёркивания «_» как признаки смыслового выделения текста:

 - Текст, окружённый одиночными «*» или «_», будет заключен в HTML-тэг `<em>`.
 -  Текст, окружённый двойными «*» или «_», будет заключен в HTML-тэг `<strong>`.

Иными словами, текст, окруженный одинарными символами, выделяется курсивным шрифтом, а текст, окруженный двойными символами, выделяется полужирным шрифтом. 
Также, выделенный фрагмент может находиться в любой части слова. 
Текст, выделенный курсивом с использованием синтаксиса языка Markdown, выглядит следующим образом:

    *Пример*  
*Пример*  

Текст, выделенный полужирным шрифтом с использованием синтаксиса языка Markdown, выглядит следующим образом:

    **Пример**
**Пример**  

Текст, выделенный курсивным полужирным шрифтом с использованием синтаксиса языка Markdown выглядит следующим образом:

    ***Пример***
***Пример***

Все приведенные выше примеры аналогичны следующим:

    _Пример_

    __Пример__

    Пере___распред___деление

    ___Пример___  

# Кодовые фрагменты строк
Чтобы отметить фрагмент строки, содержащий код, необходимо окружить его обратными апострофами «`».  При использовании кодовых фрагментов строк текст будет отображаться в виде моноширинного шрифта. 
В отличие от блоков кода, кодовый фрагмент позволяет поместить код внутрь обычного абзаца текста.
Кодовый фрагмент строки в языке Markdown выглядит следующим образом:

Используйте оператор `if`  

# Изображения
В Markdown существует 2 способа вставки изображений в документ:

a.	С помощью непосредственного указания URL-адреса изображения. Синтаксис данной команды выглядит следующим образом:

    ![Альтернативный текст](/путь/к/изображению.jpg)
или

    ![Альтернативный текст](/путь/к/изображению.jpg "Подсказка")
Иными словами, он состоит из следующих элементов:

 - восклицательный знак;
 -  квадратные скобки, в которых указывается альтернативный изображению текст (он станет содержимым атрибута в элементе img);
 -  круглые скобки, содержащие URL-адрес или относительный путь изображения, а также (необязательно) всплывающую подсказку, заключённуе в двойные или одиночные кавычки.

b.	С помощью метки-идентификатора.  Синтаксис данной команды записывается следующим образом:

    ![Альтернативный текст][id]
где «id» — имя определённой метки изображения. Метки изображений определяются при помощи синтаксиса, совершенно идентичного меткам гиперссылок:

    [id]: путь/к/изображению "Необязательная подсказка"
Важной особенностью является то, что Markdown не позволяет задать размеры изображения (ширину, высоту).  

#	Цитаты  
ля обозначения цитат в языке Markdown используется знак «больше» («>»). Его можно вставлять как перед каждой строкой цитаты, так и только перед первой строкой параграфа. 
Также синтаксис Markdown позволяет создавать вложенные цитаты (цитаты внутри цитат). Для их разметки используются дополнительные уровни знаков цитирования («>»).
Цитаты в Markdown могут содержать всевозможные элементы разметки.
Цитаты в языке Markdown выглядят следующим образом:

    >Это пример цитаты,
    >в которой перед каждой строкой
    >ставится угловая скобка.

    >Это пример цитаты,
    в которой угловая скобка
    ставится только перед началом нового параграфа.
    >Второй параграф.

Вложение цитаты в цитату выглядит следующим образом:

    > Первый уровень цитирования
    >> Второй уровень цитирования
    >>> Третий уровень цитирования
    >
    >Первый уровень цитирования
В результате на экран выводится следующее:

>Это пример цитаты,
>в которой перед каждой строкой
>ставится угловая скобка.

>Это пример цитаты,
в которой угловая скобка
ставится только перед началом нового параграфа.

>Второй параграф.

Вложенная цитата:

> Первый уровень цитирования
>> Второй уровень цитирования
>>> Третий уровень цитирования
>
>Первый уровень цитирования


Уровень цитирования не может превышать 15-й.  
# Ссылки
Markdown поддерживает два стиля оформления ссылок:

 - Гиперссылка, с немедленным указанием адреса (внутритекстовая);
 - Гиперссылка, подобная сноске.

Подразумевается, что помимо URL-адреса существует еще текст ссылки. Он заключается в квадратные скобки. 
Для создания внутритекстовой гиперссылки необходимо использовать круглые скобки сразу после закрывающей квадратной. Внутри них необходимо поместить URL-адрес. В них же возможно расположить название, заключенное в кавычки, которое будет отображаться при наведении, но этот пункт не является обязательным. 
 
      [пример](http://example.com/ "Необязательная подсказка")
В результате на экран выводится следующее:
[пример](http://example.com/ "Необязательная подсказка")
При ссылке на локальную директорию возможно использование относительного пути (от текущей страницы, сайта и т.п.)  

При создании сносной гиперссылки вместо целевого адреса используется вторая пара квадратных скобок, внутри которых помещается метка, идентификатор ссылки (id).

    [пример][id]:
Также, можно использовать пробел, чтобы отделять 2 пары квадратных скобок: 

    [пример] [id]: 

В этом случае возможно определить идентификатор в любом месте документа: 

    [id]: http://example.com/ "Необязательная подсказка"

В результате на экран выводится следующее:
[пример] [id] 
[id]: http://example.com/ "Необязательная подсказка"
Иными словами, она состоит из следующих элементов:

 - Идентификатор ссылки, окружённый квадратными скобками (которым может предшествовать необязательный отступ от одного до трёх пробелов);
 - 	Двоеточие;
 - 	Один или несколько пробелов (или символов табуляции);
 - 	URL гиперссылки;
 - 	Необязательный заголовок (подсказка к изображению, которая всплывает при наведении на него) гиперссылки, заключённый либо в двойные или одиночные кавычки, либо в скобки.

Идентификаторы ссылок могут состоять из букв, цифр, пробелов и знаков пунктуации, однако они не чувствительны к регистру. То есть эти два варианта эквивалентны:

    [текст ссылки][a]
    [текст ссылки][A]
Markdown позволяет также использовать неявно выраженный идентификатор (сокращенный). В этом случае метка не приводится, вместо неё текст гиперссылки используется  и в качестве её имени, а вторая пара квадратных скобок остаётся пустою.
Например, чтобы сделать слово «Example» гиперссылкой, ведущей на сайт <http://example.com/>, достаточно написать:

    [Example][]
и затем определить гиперссылку:

    [Example]: http://example.com/
В результате на экран выводится следующее:
[Example][]
[Example]: http://example.com/  

# Блоки кода
Отформатированные блоки кода используются в случае необходимости процитировать исходный код программ или разметки. 
Для создания блока кода в языке Markdown необходимо каждую строку параграфа начинать  с отступа, состоящего из четырех пробелов или  одного символа табуляции. Блок кода продолжается до тех пор, пока не встретится строка без отступа (или конец текста).  Внутри блока кода амперсанды («&») и угловые скобки («<» и «>») автоматически преобразуются в элементы HTML разметки. Кроме того, следует отметить, что внутри блоков кода обычный синтаксис Markdown не обрабатывается. 
Блок кода в Markdown выглядит следующим образом:

Это обычный параграф:

	Это блок кода
Дополнительные элементы
-------------------------  

# Обратный слеш
Может употребляться в Markdown перед специальными символами для того, чтобы они воспринимались в их буквальном (а не служебном) значении. Полный список данных символов приводится ниже:

«\»  - слеш;  

«`»  - обратный апостроф;  

«*»  - звездочка;  

«_»  - символ подчеркивания;  

«{}»  - фигурные скобки;  

«[]»  - квадратные скобки;  

«()»  - круглые скобки;  

«#»  - символ решетки;  

«+»  - плюс;  

«-»  - минус (дефис);  

«.»  – точка;  

«!»  - восклицательный знак.  

# Автоматические ссылки
Markdown поддерживает упрощённый порядок автоматического создания ссылок для URL-адресов и адресов электронной почты. Для этого достаточно поместить URL-адрес или почтовый адрес в угловые скобки, и Markdown сделает его гиперссылкой. В отличие от вышеописанных стилей, в данном случае сам же URL-адрес или почтовый адрес становится и текстом гиперссылки. Автоматические ссылки на адреса электронной почты работают аналогично.
Автоматические ссылки в языке Markdown выглядят следующим образом

    <http://example.com/>
В результате на экран выводится следующее:
<http://example.com/>

Автоматическая ссылка на адрес электронной почты в Markdown выглядит следующим образом

    <address@example.com>
В результате на экран выводится следующее:
<address@example.com>  

#  Специальные символы HTML
В языке HTML существует два символа, требующих специального рассмотрения: это символы («&lt;») и («&amp;»). Левая угловая скобка используется как начало тэга; амперсанды применяются для обозначения специального символа HTML.
Для того чтобы использовать эти символы в их буквальном смысле, необходимо заменить их элементами HTML, а именно `&lt;` и `&amp;` соответственно.
При использовании Markdown подобных действий совершать не нужно. Он позволяет использовать эти символы в исходном виде. В случае если амперсанд используется как часть спецсимвола HTML, он останется неизменным. В противном случае Markdown преобразует его в `&amp;`. 
