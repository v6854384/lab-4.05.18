B::foo()B::bar()A::baz()C::foo()C::bar()A::baz()

выделяем память для а1
так как фунуция baz не помечена виртуалом, то таблица виртуальных методов будет состоять только из двух ячеек:

B::foo()B::bar()

далее выделяем память для а2

функция bar обозначена виртуалом в базовом классе, поэтому обращается к таблице виртуальных методов и затем переопределяются значения в этой таблице
функция  baz не определана виртуалом, поэтому в таблице методов ничего не переопределяется

таблица методов для последних трех функций

C::foo()С::bar()A::baz()
