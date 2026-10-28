# Сторонние компоненты

Код ChessPilot (правила шахмат, связь с движком, распознавание доски, управление мышью, интерфейс) написан для ChessPilot и закрыт. В сборку входят отдельные компоненты других авторов. Каждый остаётся под своей лицензией, а тексты лицензий лежат в папке `licenses` архива программы.

| Компонент | Где в сборке | Лицензия | Исходники |
|---|---|---|---|
| **Stockfish 19**, шахматный движок. Отдельная программа, ChessPilot общается с ней по UCI | `_internal/engine/stockfish.exe` | GPL-3.0 | `_internal/engine/stockfish-source`, архив `Stockfish-19-source.zip` в каждом релизе, [официальный репозиторий sf_19](https://github.com/official-stockfish/Stockfish/tree/sf_19) |
| **Qt 6, PySide6, Shiboken6**. Отдельные библиотеки, их можно заменить совместимой сборкой | `_internal/PySide6`, `_internal/shiboken6` | LGPL-3.0 / GPL-3.0 | [code.qt.io](https://code.qt.io), [Qt for Python](https://download.qt.io/official_releases/QtForPython/) |
| **Изображения фигур** © Colin M. L. Burnett, изменены только цвета | `_internal/assets/pieces` | GFDL / BSD / GPL на выбор, используется BSD | [Wikimedia Commons](https://commons.wikimedia.org/wiki/Category:SVG_chess_pieces) |
| **Python 3.12** | `_internal` | PSF License | [python.org](https://www.python.org/downloads/source/) |
| **NumPy** | `_internal/numpy` | BSD-3-Clause | [numpy.org](https://numpy.org) |
| **Pillow** | `_internal/PIL` | MIT-CMU | [python-pillow.org](https://python-pillow.org) |
| **PyWinRT** | `_internal/winrt` | MIT | [github.com/pywinrt](https://github.com/pywinrt/pywinrt) |
| **Загрузчик PyInstaller** | `ChessPilot.exe` | GPL-2.0 с исключением: собранные программы можно распространять на любых условиях | [pyinstaller.org](https://pyinstaller.org/en/stable/license.html) |
