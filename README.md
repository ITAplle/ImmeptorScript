# TBot
TBot - это язык программирования, созданный для облегчения написания Телеграм ботов.

Чтобы начать работать, вам нужно:
1. Скачать библиотеку Python командой: `pip install tbot`
2. Создать папку, которая будет проектом, её вид должен быть следующий:
  * <папка>:
    * TestBot
      * main.tb
    * main.py
3. В файле `main.tb` записывается код на выполнение, запишите туда:
```tb
WHEN MESSAGE IS "Hello" {
  SEND TEXT "Hello, User!"
}
```
4. В файле `main.py` напишите:
```python
from tbot.TBot import TBot

TBot(
  token="",  # токен, полученный от BotFather
  path="/TestBot"    # путь до папки с проетом TBot
)
```
5. Запустите `main.py`
