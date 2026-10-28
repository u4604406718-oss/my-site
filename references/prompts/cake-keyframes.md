# Клубничный торт: кадры-ключи и видео «как пицца»

Схема — как в `pizza-higgsfield-video.md`: 4 картинки-ключа → один непрерывный ролик 10–12 с.
Исходник: фото торта Ирины (красный фон, крем, клубника, летящие ягоды), загружено в Higgsfield, media_id
`2cb28ab5-bab4-45dd-ad98-7273101e03a2` (ссылка для загрузки действует сутки; потом загрузить фото заново).

Модель для картинок: **GPT Image 2.5** (`gpt_image_2_5`), качество high, 3:2 — **1,5 кредита за картинку**
(FLUX 3 — 2 кредита). 4 кадра ≈ 6 кредитов + видео.
Все 4 кадра генерировать **в одной сессии**, каждый с исходным фото как референсом.

## Сюжет
целый торт → поднимается и вращается → **разлетается на слои** → слои падают обратно и собираются → торт опускается на подставку → финальный кадр с кусочком.

## Кадр 1 — старт (чистый герой)
```
Use the uploaded image as the exact reference for the cake, colours, lighting and background.
A whole layered strawberry cream cake standing perfectly on a glossy red cake stand, centred, against the same deep red gradient background.
No flying strawberries yet, clean calm composition, a few tiny cream droplets only.
Same warm soft studio lighting, same camera angle, premium food commercial photography, 3:2.
Do not add text, logos, people or new objects. Do not redesign the cake.
```

## Кадр 2 — взрыв на слои (пик)
```
Use the uploaded image as the exact reference for the cake, colours, lighting and background.
The same strawberry cream cake deconstructed in mid-air into distinct floating horizontal layers, stacked vertically with clear gaps:
bottom sponge → cream → sliced strawberries → sponge → cream → whole and halved strawberries on top.
Cream stretches naturally between layers, glossy strawberry sauce drips and droplets, strawberry slices flying outward with energy.
The red cake stand stays below, empty. Same deep red background, same warm lighting, same camera angle.
Premium food commercial photography, controlled cinematic explosion, sharp focus, 3:2.
Do not add text, logos, people or new ingredients.
```

## Кадр 3 — сборка и приземление
```
Use the uploaded image as the exact reference for the cake, colours, lighting and background.
The layers of the strawberry cream cake falling back together and landing on the glossy red cake stand,
the cake almost fully reassembled, last strawberries dropping onto the top, a soft splash of cream and sauce droplets at the moment of impact.
Same deep red background, same warm lighting, same camera angle, slight motion blur on the falling pieces.
Premium food commercial photography, 3:2. Do not add text, logos, people or new objects.
```

## Кадр 4 — финал (продающий)
```
Use the uploaded image as the exact reference for the cake, colours, lighting and background.
The finished strawberry cream cake on the glossy red cake stand with one perfect slice cut and slightly pulled out,
showing the clean layers of sponge, cream and strawberries inside. A few strawberries resting around the stand.
Same deep red background, calm and appetizing, warm soft studio lighting, same camera angle.
Premium food commercial photography, hero shot, 3:2. Do not add text, logos or people.
```

## Видео по кадрам (после того как 4 кадра готовы)
```
Using Higgsfield create a dynamic cinematic dessert commercial using the 4 uploaded reference images as strict sequential keyframes.
IMAGE 1 → IMAGE 2 → IMAGE 3 → IMAGE 4. ONE continuous seamless shot: no cuts, no fades, no black frames.

IMAGE 1 — START: begin exactly from Image 1. The cake slowly rotates on the stand, then lifts into the air, rotation speeding up,
the camera moves closer and subtly orbits.
IMAGE 1 → IMAGE 2 — EXPLOSION: in mid-air the cake deconstructs into floating layers (sponge, cream, strawberries),
cream stretches before separating, strawberry slices and sauce droplets fly outward. Controlled cinematic explosion, not a cut.
At the peak recreate Image 2 as closely as possible.
IMAGE 2 → IMAGE 3 — REASSEMBLY: the layers reverse and fall back together onto the stand, strawberries drop onto the top,
soft splash of cream on impact. Match Image 3.
IMAGE 3 → IMAGE 4 — FINAL: the camera slowly pushes in, a slice separates and slides out showing the layers. End exactly on Image 4.

Style: high-end dessert commercial, realistic food physics, glossy sauce, soft cream, warm light, rich deep red tones,
smooth camera, subtle motion blur, never shaky. Keep the cake, stand and background consistent with the references.
Do NOT add text, people, new ingredients or environments.
Duration about 10 seconds, aspect ratio 16:9.
```

## Для сайта
- Видео → кадры для canvas (`patterns.md`, «Движок видео по скроллу» и «Загрузка кадров»).
- Если первый и последний кадр должны совпадать (зацикливание) — добавить в промпт видео: `first and last frames must be identical`.
- Отличие от клубничного сайта: теперь есть сценарий из 4 ключей, а не «вслепую».
