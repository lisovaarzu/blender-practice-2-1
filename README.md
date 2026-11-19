# Практика 2.1 — выборочная доработка UV для проверки

Это отдельная версия для сравнения, сохранённая в новой ветке `uv-revision-review`. Первоначальный комплект в ветке [deliverables-v2.0](https://github.com/lisovaarzu/blender-practice-2-1/tree/deliverables-v2.0), main и Releases не заменены.

## Скачать новый компактный комплект

- [Часть 001 — 70.00 МиБ](https://raw.githubusercontent.com/lisovaarzu/blender-practice-2-1/refs/heads/uv-revision-review/Download/Practice_2_1_UV_Revision.zip.001)
- [Часть 002 — 69.83 МиБ](https://raw.githubusercontent.com/lisovaarzu/blender-practice-2-1/refs/heads/uv-revision-review/Download/Practice_2_1_UV_Revision.zip.002)

Скачайте обе части в одну папку с исходными именами. В cmd выполните:

```cmd
copy /b Practice_2_1_UV_Revision.zip.001+Practice_2_1_UV_Revision.zip.002 Practice_2_1_UV_Revision.zip
```

Распакуйте ZIP в **отдельную новую папку**, не поверх Before. Откройте `Practice_2_1/Practice_2_1_Final.blend` в Blender 5.3.0.

Внутри ровно восемь файлов: .blend, FBX, Normal_Map.png, Base_Color.png, UV_Layout.png, Shader_Nodes.png, Render_Final.png, Work_Steps.md. Before, дополнительные ракурсы, Checker, сетка, промежуточные версии и технические JSON не включены.

[Подробный отчёт](Work_Steps.md) · [Инструкция для Windows](Download/Windows_README_RU.txt) · [SHA256](Download/SHA256SUMS.txt)

## Проверки

| Показатель | Before | После |
|---|---:|---:|
| UV-острова | 3088 | 2530 |
| Острова из 1–3 граней | 2697 | 2063 |
| Острова площадью <64 пикселей² | 19 | 0 |
| Заполнение UV | 35,66% | 31,35% |
| Минимальный зазор при 4096² | 8,16 px | 16,03 px |
| Растяжение p95 / максимум | 1,478 / 2,204 | 1,478 / 2,204 |
| Треугольники | 8874 | 8874 |
| Перекрытия / выход за 0–1 | 0 / 0 | 0 / 0 |

Геометрия, камера, свет и настройки материала сохранены. Normal Map и Base Color запечены заново; ошибочная первая проба рендера отклонена и исправлена геометрическим переносом нормалей с High Poly. Финальные изображения получены в Blender. Проверены FBX после повторного импорта и открытие перемещённой копии .blend без внешних текстур. Изображения упакованы, пути относительные. Новая версия непосредственно на Windows не запускалась.

Это выборочная доработка: островов всё ещё много. Заполнение карты уменьшено ради отступов; внешний вид проверен при неизменных настройках сцены. Подробные ограничения — в отчёте.

SHA256 восстановленного ZIP: `c7ec046e679db4178122569c5315017e3c33df299617f4f4ac47f7d7f5eba869`.

Исходник: Stoneware Whisky Flagon in Wicker Basket, Global Digital Heritage and GDH-Afrika, CC-BY-NC-4.0. Полное указание авторства и ссылка приведены в отчёте.
