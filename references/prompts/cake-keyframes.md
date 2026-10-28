# Клубничный торт: кадры-ключи и видео «как пицца»

Схема — как в `pizza-higgsfield-video.md`: 4 картинки-ключа → один непрерывный ролик ~10 с.
Исходник: фото торта Ирины (красный фон, крем, клубника, летящие ягоды, красная подставка).

## Что меняем относительно исходного фото (решение от 28.10.2026)

| Было | Стало | Почему |
|---|---|---|
| Красный торт на красном фоне | **Контрастный фон** (см. ниже) | Красная клубника сливается с красным фоном, теряется объём. У пиццы фон тоже одного тона, но корж и сыр жёлто-белые и отделяются от оранжевого; у торта такого разделения нет. |
| Торт на красной подставке | **Торт парит в воздухе** | Как пицца: ничто не мешает «взрыву» на слои, кадр чище, на сайте торт можно вырезать и поставить где угодно. Подставка — лишний предмет, который тоже надо анимировать. |
| — | ~~Финал: торт в открытой коробке кондитерской на столе~~ | **Отменено 28.10.2026 после пробы:** стол и белая коробка выглядят дёшево, появилась «стена с горизонтом» вместо студийного фона. Ирине не понравилось. |
| — | **Финал: торт собирается и остаётся парить в той же фисташковой студии, потом отделяется кусочек** | Один бесшовный фон на весь ролик = премиально (правило шаблона фото товаров: «no props, no floor»; визуал референсов: продукт на чистом фоне). Сайт сам «продаёт» кнопкой, коробка в кадре не нужна. |

**Урок для агента:** промпт пиццы рассчитан на бренд с узнаваемой коробкой (Додо). Без фирменной упаковки «коробка + стол» превращаются в дешёвый реквизит. Финал брать из логики продукта: у торта самое вкусное — разрез со слоями.

### Фон — три варианта (выбрать один, вставить вместо `[BACKGROUND]`)
1. ✅ **Выбран 28.10.2026. Фисташковый / мятный:** `soft pistachio green gradient background, #B9D8B0 to #8FBF8A`.
   Зелёный — противоположность красного: клубника «горит», белый крем отделяется. Свежо и ярко, как оранжевый у пиццы.
2. **Пудрово-розовый («клубничное молоко»):** `soft blush pink gradient background, #F6D6D6 to #EDB9BE`.
   Нежно и «женственно», тот же цветовой мир, но крем и ягоды читаются.
3. **Шоколадный:** `deep warm chocolate brown gradient background, #4A2C21 to #2B1912`.
   Премиально и «вкусно», красный и белый очень контрастны. Для дорогой кондитерской.

Фон сайта потом = фон видео (тот же цвет), чтобы торт «стоял» прямо на странице.


## ✅ Финал v3 (28.10.2026, решение Ирины): красивая коробка, без дешёвого стола
Кадры 1 и 2 готовы. Кадр 3 с белой коробкой на деревянном столе — дёшево. Кадр 4 с отрезанным кусочком — торт «нарезан ровными кусками», не понравилось.
Решение: **коробка остаётся, но премиальная**, стоит на бесшовном фисташковом «полу» той же студии (без стола и горизонта).
Финал как у пиццы — **закрытая коробка**, без разреза торта.

### Кадр 3 v3 — торт опускается в открытую коробку
```
Use the uploaded image as the exact reference for the cake, cream, strawberries, background colour and lighting.
The same whole strawberry cream cake gently lands inside an open premium rigid gift box: matte cream-white box with a thin pistachio green rim,
the lid standing open behind it, a pistachio satin ribbon lying loosely beside the box.
The box stands on a seamless pistachio green studio surface that curves smoothly into the same soft pistachio gradient background —
no table, no wood, no wall, no horizon line. The last two strawberries are still dropping onto the top, a tiny soft splash of cream.
Warm soft studio light from upper left, soft natural shadow under the box. Camera slightly above, about 20 degrees.
Luxury patisserie commercial photography, 3:2. The cake stays whole, not sliced. Box completely blank, no text, no logos, no people.
```

### Кадр 4 v3 — закрытая коробка с лентой (финал)
```
Use the uploaded image as the exact reference for the box, ribbon, background and lighting.
The same premium matte cream-white gift box with thin pistachio rim, now closed with its lid, tied with the pistachio satin ribbon in a neat bow.
Two fresh strawberries and a small swirl of cream rest next to the box on the same seamless pistachio studio surface,
same soft pistachio gradient background, no table, no horizon line. Calm luxury hero shot, warm soft light from upper left.
Luxury patisserie commercial photography, 3:2. Box completely blank, no text, no logos, no people.
```
Кадр 3 v3 делать с **кадром 1** как референсом; кадр 4 v3 — с **кадром 3 v3** (чтобы коробка была та же).
Видео: `… layers reassemble → the cake lands in the open box → the lid closes → the ribbon ties → final closed-box hero shot.`

## Бесплатное видео: три перехода «первый → последний кадр» (28.10.2026)
Бесплатные генераторы с режимом «start frame + end frame» (Kling, Luma Dream Machine, LTX, Google Flow) делают ролик
**между двумя картинками**, 5–10 с. Поэтому делаем **три коротких клипа** и склеиваем:
`1-floating → 2-explosion`, `2-explosion → 3-box-open`, `3-box-open → 4-box-closed`.
Конец клипа = начало следующего, поэтому склейка незаметна. Склеить — ffmpeg (агент сделает), бесплатно.
На бесплатных тарифах обычно водяной знак и 720p — для учёбы и пробы нормально.

### Клип A: 1 → 2 (взрыв)
```
The floating strawberry cream cake slowly rotates, then lifts slightly and bursts apart into separate floating layers:
sponge, cream, strawberries. Cream stretches before separating, sauce droplets and strawberry slices fly outward.
Smooth cinematic motion, camera slowly pulls back a little. Same pistachio studio background. No cuts.
```
### Клип B: 2 → 3 (сборка и падение в коробку)
```
The floating layers fall back together into the whole cake, which gently descends and lands inside an open cream-white gift box,
the last strawberries drop onto the top with a soft splash of cream. Camera follows smoothly and tilts down slightly.
Same pistachio studio background. No cuts.
```
### Клип C: 3 → 4 (крышка и бант)
```
The lid of the gift box closes smoothly over the cake, the pistachio satin ribbon wraps around the box and ties into a neat bow.
Camera slowly pushes in. Calm, elegant motion. Same pistachio studio background. No cuts.
```

## Модель и стоимость
- Higgsfield: GPT Image 2.5, high, 3:2 — 1,5 кредита за кадр (на 28.10.2026 кредитов 0).
- **Бесплатно:** ChatGPT или Gemini. Все 4 кадра делать **в одном чате**, к каждому прикладывать исходное фото торта.

## Сюжет
торт парит и медленно вращается → **разлетается на слои** → слои собираются обратно в воздухе → камера приближается, отделяется кусочек. Весь ролик в одной фисташковой студии.

## Кадр 1 — старт (торт парит)
```
Use the uploaded image as the exact reference for the cake: same layers, cream, strawberries and sauce.
Remove the cake stand completely. The whole layered strawberry cream cake floats in mid-air, centred, slightly tilted toward the camera,
on a clean [BACKGROUND]. Only a few small strawberry slices and cream droplets float around it.
Warm soft studio lighting from upper left, soft shadow below the cake, premium food commercial photography, 3:2.
Do not add text, logos, people, a plate or a stand. Do not redesign the cake.
```

## Кадр 2 — взрыв на слои (пик)
```
Use the uploaded image as the exact reference for the cake, cream and strawberries.
No cake stand. The same strawberry cream cake deconstructed in mid-air into distinct floating horizontal layers stacked vertically with clear gaps:
bottom sponge → cream → sliced strawberries → sponge → cream → whole and halved strawberries on top.
Cream stretches naturally between layers, glossy strawberry sauce drips and droplets, strawberry slices flying outward with energy.
Same [BACKGROUND], same warm lighting and camera angle as the previous image.
Premium food commercial photography, controlled cinematic explosion, sharp focus, 3:2.
Do not add text, logos, people or new ingredients.
```

## Кадр 3 — сборка (торт снова целый, парит)
```
Use the uploaded image as the exact reference for the cake, cream, strawberries, background and lighting.
The layers of the same strawberry cream cake have just snapped back together in mid-air: the cake is whole again and floats in the same position,
the last few strawberries are still dropping onto the top, a small soft splash of cream and a few sauce droplets around the top edge.
Same seamless soft pistachio green gradient studio background, no table, no floor, no box, no stand, no horizon line.
Same warm soft light from upper left, soft shadow far below, slight motion blur only on the falling strawberries.
Premium food commercial photography, 3:2. Do not add text, logos, people or props. Do not change the cake design.
```

## Кадр 4 — финал (разрез со слоями)
```
Use the uploaded image as the exact reference for the cake, cream, strawberries, background and lighting.
The same whole strawberry cream cake floats calmly in mid-air; one perfect triangular slice has separated and floats slightly out toward the camera,
showing clean layers of sponge, cream and strawberries inside. Two or three strawberry halves float nearby.
Same seamless soft pistachio green gradient studio background, no table, no floor, no box, no stand.
Calm, appetizing, warm soft studio light from upper left, gentle shadow far below. Premium food commercial photography, hero shot, 3:2.
Do not add text, logos, people or props.
```

## Видео по кадрам (когда 4 кадра готовы, в Higgsfield)
```
Create a dynamic cinematic dessert commercial using the 4 uploaded reference images as strict sequential keyframes.
IMAGE 1 → IMAGE 2 → IMAGE 3 → IMAGE 4. ONE continuous seamless shot: no cuts, no fades, no black frames.

IMAGE 1 — START: begin exactly from Image 1. The floating cake slowly rotates in mid-air, the rotation speeds up,
the camera moves closer and subtly orbits.
IMAGE 1 → IMAGE 2 — EXPLOSION: the cake deconstructs into floating layers (sponge, cream, strawberries),
cream stretches before separating, strawberry slices and sauce droplets fly outward. Controlled cinematic explosion, not a cut.
At the peak recreate Image 2 as closely as possible.
IMAGE 2 → IMAGE 3 — REASSEMBLY: the layers reverse and snap back together in mid-air, the last strawberries drop onto the top
with a soft splash of cream. The cake stays floating in the same seamless pistachio studio. Match Image 3.
IMAGE 3 → IMAGE 4 — FINAL: the camera slowly pushes in, one slice separates and floats out toward the camera showing the layers. End exactly on Image 4.

Style: high-end dessert commercial, realistic food physics, glossy sauce, soft cream, warm light,
the same background colour throughout, smooth camera, subtle motion blur, never shaky.
Do NOT add text, people, new ingredients, tables, boxes or environments. Do NOT redesign the cake.
Duration about 10 seconds, aspect ratio 16:9.
```

## Сверка с готовыми промптами и инструкциями

| Источник | Что взято в промпты торта | Где |
|---|---|---|
| **Промпт пиццы** (`pizza-higgsfield-video.md`) | 4 кадра-ключа «строго по порядку»; ONE continuous shot без склеек; каждый переход описан физикой (вращение → взрыв на слои → обратная сборка → падение в коробку); крем тянется перед разделением, как сыр у пиццы; камера «живая»: push-in, orbit, но не трясётся; запреты в конце; «не менять продукт и упаковку»; цепочка `A → B → C` в конце | все кадры и видео |
| **Пицца: чего у торта не было** | «subtle steam and realistic food particles» → у торта: капли соуса и крема; финал пиццы — **закрытая коробка**: даю как вариант кадра 4 (см. ниже) | кадры 2–4 |
| **Шаблон фото товаров** (из часов Ora, `product-photo-template.md`) | однотонный градиентный фон без пола и предметов; свет «soft large-source from upper left»; «no props, no text, no logos»; **все кадры в одной сессии, одним стилем**; таблица исправлений (ниже) | кадр 1, правила |
| **Кофейня BREWNS** (`knowledge/prompts/coffee-brewns.md`) | фон видео = фон блока сайта; один акцентный цвет; **предметы летают вокруг продукта** (у них зёрна, у нас ломтики клубники) | фон, кадры 1–2 |
| **Схема персонажа Higgsfield** | для зацикленного видео по скроллу: «first and last frames must be identical» | вариант видео (ниже) |
| **Marlin / Orven** (`water-marlin.md`, `sunglasses-orven.md`) | генерация даёт ~10 с → если нужно длиннее, два клипа со стыком «последний кадр = первый кадр» | видео |
| **visual.md + copy.md** | герой крупно по центру, заголовок «утверждение + поворот», один акцент | для сайта |

### ~~Вариант финала «как у пиццы» (кадр 4б — закрытая коробка)~~ — отклонён: только для бренда с фирменной премиальной упаковкой
```
Use the uploaded image as the exact reference for the cake.
The same white pastry box on the light wooden table, now closed, a few fresh strawberries and a little cream on the table next to it,
[BACKGROUND] behind, warm soft studio light, calm final hero shot, premium food commercial photography, 3:2.
Do not add text, logos or people.
```
В видео тогда последняя строка цепочки: `… lands in the open box → box rotates slightly → lid closes → final closed-box hero shot.`

### Если кадр «уехал» (дописать в конец промпта)
| Проблема | Добавить |
|---|---|
| Подставка всё равно появилась | `no cake stand, no plate, the cake floats in mid-air` |
| Фон снова красный / не тот | `pure smooth [BACKGROUND], no red background` |
| Торт стал другим | `keep the exact same cake design, layers and strawberry placement as the reference` |
| Торт мелкий | `the cake fills about 60 percent of the frame height` |
| Появились буквы на коробке | `completely blank box, no lettering anywhere` |
| Слишком много летающих ягод (кадр 1) | `only 3–5 small strawberry slices around, calm composition` |

### Для зацикливания на сайте (по скроллу туда-обратно)
Если торт нужен как бесконечное вращение в герое — отдельное короткое видео из кадра 1:
`The floating cake slowly rotates 360 degrees in place, camera locked, first and last frames must be identical.`

## Для сайта
- Видео → кадры для canvas (`patterns.md`, «Движок видео по скроллу» и «Загрузка кадров»).
- Текст героя по формуле «утверждение + поворот», например: «Это не просто торт. / Это клубника, которую ждёшь всё лето».
- Отличие от клубничного сайта: сценарий из 4 ключей, контрастный фон, без лишних предметов.
