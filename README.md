# module_20
Программа демонстрирует пересылку сообщений, адресованных всем пользователям чата, на сервер.
Для проверки работоспособности нужно:
1) запустить программу-сервер (в папке testServer)
2) запустить 2 экземпляра программы-чат
3) создать в чате-1 и чате-2 пользователей и зайти под ними
4) в чате-1 выбрать "to write a message", далее ввести "all", далее ввести сообщение без пробелов. После нажатия Enter сообщение попадет на сервер (распечатается)
5) повторить пункт 4 для чата-2

К сожалению, я не успел разобраться как переслать сообщение от одного конкретного пользователя другому. Для этого необходимо производить сеарилизацию и десеарилизацию объекта сообщения, что я пока не умею.
Также программа ограничена по количеству подключений (2). Но это легко меняется в коде программы-сервер.
Еще одно существенное ограничение - сервер сначала ждет подключения всех пользователей, а только потом позволяет пересылать сообщения строго по очереди.
