# Пицца: рекламный ролик из 4 фото (Claude + Higgsfield MCP)

Источник: инструкция из Instagram-поста, сохранена как пример для обучения.
Это ролик для пиццерии с видео IMG_6999 (приём «Разбор предмета на слои»).

## Схема

1. Подключить Higgsfield к Claude через MCP.
2. Подготовить 4 кадра-ключа (в оригинале сгенерированы в ChatGPT):
   1) готовая пицца на оранжевом градиенте;
   2) пицца в воздухе, разобранная на слои (основа, соус, сыр, пепперони);
   3) пицца в открытой коробке на деревянном столе;
   4) закрытая коробка, финальный кадр.
3. Отправить в Claude 4 картинки и промпт ниже. Готовое видео приходит меньше чем через минуту.

Схема подходит для любого продукта: косметики, одежды, еды, украшений.

## Промпт

```
Using Higgsfield Create a dynamic cinematic food commercial using the 4 uploaded reference images as strict sequential keyframes.

IMPORTANT: Follow the visual sequence exactly:
IMAGE 1 → IMAGE 2 → IMAGE 3 → IMAGE 4.

The entire video must feel like ONE continuous seamless shot. No cuts, no fades, no black frames, no abrupt scene changes. Every scene must naturally transform into the next one through physical movement of the pizza, ingredients, camera and box.

### IMAGE 1 — START

Begin exactly from Image 1: a finished pepperoni pizza centered against the vivid orange gradient background.

The pizza slowly rotates at first, then the rotation becomes faster and more energetic. The pizza slightly lifts into the air while the camera dynamically moves closer and subtly circles around it.

Keep the pizza appearance, crust, cheese, pepperoni, lighting and orange background consistent with the reference.

### IMAGE 1 → IMAGE 2 — EXPLOSION

While the pizza is spinning in mid-air, smoothly transition into Image 2.

The pizza dynamically deconstructs in mid-air.

Its ingredients separate vertically into distinct floating layers:
pizza base → tomato sauce → melted shredded cheese → pepperoni slices.

Pepperoni pieces fly upward with energetic momentum. Cheese stretches naturally before separating. Add subtle steam and realistic food particles.

The movement should feel like a controlled cinematic explosion, NOT a sudden cut.

At the peak of the movement, recreate the composition of Image 2 as closely as possible.

### IMAGE 2 → IMAGE 3 — REASSEMBLY AND FALL

After briefly floating in the air, all ingredients reverse their movement.

Pepperoni slices fall downward onto the cheese.
The cheese layer falls onto the tomato sauce.
The sauce settles onto the pizza base.

The pizza rapidly reassembles into the same finished pepperoni pizza from Image 1.

As soon as it becomes complete, gravity pulls the entire pizza downward.

The camera follows the pizza in one continuous fluid movement.

The orange studio environment naturally transforms into the warm wooden-table environment from Image 3.

An OPEN pizza box appears underneath.

The finished pizza falls perfectly into the center of the open box with a satisfying soft impact.

End this movement matching Image 3: open cardboard pizza box, pizza inside, warm wooden table, orange background, warm cinematic lighting.

### VISUAL & MOTION STYLE

High-end cinematic food commercial, energetic advertising style, realistic food physics, appetizing melted cheese, glossy pepperoni, realistic steam, smooth camera movement, subtle motion blur, dramatic warm lighting, rich orange tones, premium commercial photography.

The camera should constantly feel alive: subtle push-ins, orbiting movement and tracking, but never chaotic or shaky.

Maintain visual continuity between all 4 reference images.

Do NOT introduce additional ingredients, objects, text, people or environments.

Do NOT redesign the pizza or packaging.

Preserve the Dodo Pizza box design from the reference images.

ONE CONTINUOUS SEAMLESS VIDEO:
finished pizza → spinning pizza → ingredients explode into layers → ingredients fall back together → pizza reassembles → pizza falls into open box → box rotates slightly → lid closes → final closed-box hero shot.

Duration: approximately 10–12 seconds.
Aspect ratio: 16:9.
Fast, dynamic, smooth, cinematic commercial pacing
```

## Что взять в агента (обобщённо)

- **Кадры-ключи → один непрерывный план.** Заранее задаём 3–4 картинки (начало, пик, приземление, финал) и требуем «ONE continuous shot, no cuts».
- **Каждый переход описан физикой**: вращение → взрыв на слои → обратная сборка → падение в упаковку. Никаких «появляется».
- **Запреты в конце промпта:** не добавлять объекты и текст, не менять продукт и упаковку.
- **Цепочка одной строкой** в конце (`A → B → C → …`) дублирует сценарий, чтобы модель не потеряла порядок.
- Внимание: в оригинале упаковка реального бренда (Dodo Pizza). Для своих работ и продажи нужна своя упаковка или упаковка клиента.
