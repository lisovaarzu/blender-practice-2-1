# Практика 2.1 — готовые файлы

Готовый комплект кувшина в плетёной корзине: Blender 5.3.0, 8874 триса, 0 n-gon.

Файлы переданы в отдельной ветке `deliverables-v2.0` через обычный Git. Это альтернативная передача полного комплекта, а не Release Assets: загрузка в черновик v2.0 через uploads.github.com вернула HTTP 401 даже для README размером 1339 байт. Исходный v1.0 и main не изменены.

## Скачать полный комплект

Скачайте четыре части по ссылкам ниже (на странице файла при необходимости нажмите Download raw file).

- [Часть 001](https://raw.githubusercontent.com/lisovaarzu/blender-practice-2-1/refs/heads/deliverables-v2.0/Download/Practice_2_1_Complete.zip.001)
- [Часть 002](https://raw.githubusercontent.com/lisovaarzu/blender-practice-2-1/refs/heads/deliverables-v2.0/Download/Practice_2_1_Complete.zip.002)
- [Часть 003](https://raw.githubusercontent.com/lisovaarzu/blender-practice-2-1/refs/heads/deliverables-v2.0/Download/Practice_2_1_Complete.zip.003)
- [Часть 004](https://raw.githubusercontent.com/lisovaarzu/blender-practice-2-1/refs/heads/deliverables-v2.0/Download/Practice_2_1_Complete.zip.004)

Первые три части по 70 МиБ, четвёртая — 37,86 МиБ. Не открывайте их по отдельности.

[Инструкция для Windows](Download/Windows_README_RU.txt) · [SHA256](Download/SHA256SUMS.txt) · [Подробный отчёт](Work_Steps.md)

В cmd из папки с четырьмя частями выполните:

```cmd
copy /b Practice_2_1_Complete.zip.001+Practice_2_1_Complete.zip.002+Practice_2_1_Complete.zip.003+Practice_2_1_Complete.zip.004 Practice_2_1_Complete.zip
```

Ожидаемый SHA256 ZIP: `58c9b8d9318da9ba9165c2ffb0c0575225565194029e662b4bbf0f7067a09adf`.
Распакуйте ZIP и откройте `Practice_2_1/Blender/Practice_2_1_Final.blend`.

Внутри полный комплект: .blend с оригинальной High Poly и готовой Low Poly, FBX, упакованные и отдельные текстуры, запечённая Normal Map, UV/Checker/Nodes, рендер, сравнение, сетка, дополнительные ракурсы, отчёт и протоколы проверок. Нативное открытие на Windows не проверялось. Подробные ограничения сетки и UV описаны в отчёте.

![Финальный рендер](Render_Final.png)
