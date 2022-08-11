# Tests_Labirint
Репозиторий содержит пример тестирования сайта https://www.labirint.ru/ с использованием паттерна PageObject с Selenium и Python (PyTest + Selenium).
За основу я взяла шаблон, предоставленный в процессе обучения Тимуром Нурлыгаяновым. Выражаю ему за это огромную благодарность. 
В скринкасте Тимур озвучивает, что файлы base.py, elements.py и conftest.py можно просто скопировать, что я и сделала. 
Непосредственно тесты придуманы мною лично.
Каждый тест сопровождается описанием и комментариями на русском языке.
Файлы:
conftest.py содержит код для отлова неудачных тестовых случаев и создания скриншота страницы в случае, если какой-либо тест не сработает. Скриншоты сохраняются в папке "screenshots".
pages/base.py содержит реализацию шаблона PageObject для Python.
pages/elements.py содержит вспомогательный класс для определения веб-элементов на веб-страницах.
pages/labirint.py содержит локаторы элементов сайта, используемых при тестировании. 
tests/test_labirint.py содержит 50 тестов для сайта онлайн-магазина "Лабиринт" (https://www.labirint.ru/).

Для запуска тестов необходимо загрузить Selenium WebDriver с https://chromedriver.chromium.org/downloads (версию, совместимую с используемым браузером)
Запускать тесты необходимо в консоли командой:
python -m pytest -v --driver Chrome --driver-path C:\ChromeDriveSelenium\chromedriver.exe tests/test_labirint.py

python -m pytest -v --driver Chrome --driver-path С:\ChromeDriveSelenium\chromedriver.exe tests\test_labirint.py
I:\piton28\proekt667\tests\test_labirint.py