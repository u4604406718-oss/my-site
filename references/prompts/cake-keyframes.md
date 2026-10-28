# Клубничный торт: кадры-ключи и видео «как пицца»

Схема — как в `pizza-higgsfield-video.md`: 4 картинки-ключа → один непрерывный ролик ~10 с.
Исходник: фото торта Ирины (красный фон, крем, клубника, летящие ягоды, красная подставка).

## Что меняем относительно исходного фото (решение от 28.10.2026)

| Было | Стало | Почему |
|---|---|---|
| Красный торт на красном фоне | **Контрастный фон** (см. ниже) | Красная клубника сливается с красным фоном, теряется объём. У пиццы фон тоже одного тона, но корж и сыр жёлто-белые и отделяются от оранжевого; у торта такого разделения нет. |
| Торт на красной подставке | **Торт парит в воздухе** | Как пицца: ничто не мешает «взрыву» на слои, кадр чище, на сайте торт можно вырезать и поставить где угодно. Подставка — лишний предмет, который тоже надо анимировать. |
| — | **Финал: торт в открытой коробке кондитерской на столе** | Как пицца в коробке: финальный кадр продаёт доставку/заказ, а не просто красивый десерт. |

### Фон — три варианта (выбрать один, вставить вместо `[BACKGROUND]`)
1. **Фисташковый / мятный (рекомендую):** `soft pistachio green gradient background, #B9D8B0 to #8FBF8A`.
   Зелёный — противоположность красного: клубника «горит», белый крем отделяется. Свежо и ярко, как оранжевый у пиццы.
2. **Пудрово-розовый («клубничное молоко»):** `soft blush pink gradient background, #F6D6D6 to #EDB9BE`.
   Нежно и «женственно», тот же цветовой мир, но крем и ягоды читаются.
3. **Шоколадный:** `deep warm chocolate brown gradient background, #4A2C21 to #2B1912`.
   Премиально и «вкусно», красный и белый очень контрастны. Для дорогой кондитерской.

Фон сайта потом = фон видео (тот же цвет), чтобы торт «стоял» прямо на странице.

## Модель и стоимость
- Higgsfield: GPT Image 2.5, high, 3:2 — 1,5 кредита за кадр (на 28.10.2026 кредитов 0).
- **Бесплатно:** ChatGPT или Gemini. Все 4 кадра делать **в одном чате**, к каждому прикладывать исходное фото торта.

## Сюжет
торт парит и медленно вращается → **разлетается на слои** → слои падают обратно и собираются → торт опускается в открытую коробку на столе → кусочек.

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

## Кадр 3 — сборка и приземление
```
Use the uploaded image as the exact reference for the cake, cream and strawberries.
The layers of the strawberry cream cake fall back together and land inside an open plain white pastry box
standing on a light wooden table; the cake is almost fully reassembled, last strawberries dropping onto the top,
a soft splash of cream and sauce droplets at the moment of impact.
The [BACKGROUND] continues behind the table. Same warm lighting, slight motion blur on falling pieces.
Premium food commercial photography, 3:2. Do not add text, logos, people or extra objects.
```

## Кадр 4 — финал (продающий)
```
Use the uploaded image as the exact reference for the cake, cream and strawberries.
The finished strawberry cream cake inside the open plain white pastry box on a light wooden table,
one perfect slice cut and slightly pulled out, showing clean layers of sponge, cream and strawberries.
A few fresh strawberries next to the box. [BACKGROUND] behind. Calm, appetizing, warm soft studio light.
Premium food commercial photography, hero shot, 3:2. Do not add text, logos or people.
```
Коробка без надписей: логотип кондитерской клиента добавляется потом (или своим брендом для портфолио).

## Видео по кадрам (когда 4 кадра готовы, в Higgsfield)
```
Create a dynamic cinematic dessert commercial using the 4 uploaded reference images as strict sequential keyframes.
IMAGE 1 → IMAGE 2 → IMAGE 3 → IMAGE 4. ONE continuous seamless shot: no cuts, no fades, no black frames.

IMAGE 1 — START: begin exactly from Image 1. The floating cake slowly rotates in mid-air, the rotation speeds up,
the camera moves closer and subtly orbits.
IMAGE 1 → IMAGE 2 — EXPLOSION: the cake deconstructs into floating layers (sponge, cream, strawberries),
cream stretches before separating, strawberry slices and sauce droplets fly outward. Controlled cinematic explosion, not a cut.
At the peak recreate Image 2 as closely as possible.
IMAGE 2 → IMAGE 3 — REASSEMBLY AND FALL: the layers reverse and fall back together, gravity pulls the whole cake down,
the camera follows, a light wooden table and an open white pastry box appear underneath, the cake lands in the box
with a soft splash of cream. Match Image 3.
IMAGE 3 → IMAGE 4 — FINAL: the camera slowly pushes in, a slice separates and slides out showing the layers. End exactly on Image 4.

Style: high-end dessert commercial, realistic food physics, glossy sauce, soft cream, warm light,
the same background colour throughout, smooth camera, subtle motion blur, never shaky.
Do NOT add text, people, new ingredients or environments. Do NOT redesign the cake or the box.
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

### Вариант финала «как у пиццы» (кадр 4б — закрытая коробка)
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
