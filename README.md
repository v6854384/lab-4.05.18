B::foo()B::bar()A::baz()C::foo()C::bar()A::baz()

Выделяем память для а1

Так как фунуция baz не помечена виртуалом, то таблица виртуальных методов будет состоять только из двух ячеек:

B::foo()B::bar()

Далее выделяем память для а2

Функция bar обозначена virtual в базовом классе, поэтому обращается к таблице виртуальных методов и затем переопределяются значения в этой таблице

Функция  baz не определана virtual, поэтому в таблице методов ничего не переопределяется

Таблица методов для последних трех функций:

C::foo()С::bar()A::baz()
