# Шаблон промпта для фото товара (Higgsfield / любой генератор)

Обобщено из промпта часов Ora (`knowledge/prompts/watch-ora.md`). Подходит для каталога: часы, украшения, косметика, обувь, техника, упаковка еды.
Заполняем скобки, остальное оставляем как есть. Пишем по-английски — генераторы понимают его лучше.

```
Ultra-detailed premium product photograph of [ЧТО: a matte black ceramic coffee cup],
single object centred on a flat [ЦВЕТ ФОНА: near-black #0A0D14] background.
[ДЕТАЛИ: материал, форма, цвет, фактура, особенности — 2–4 фразы].
Shot straight-on at a very slight three-quarter tilt.
Soft large-source studio lighting from upper left, crisp specular highlight along the [ГДЕ БЛИК: rim / polished edge],
controlled reflections, no blown highlights.
Razor-sharp focus on [ГЛАВНОЕ: the logo area / the dial / the texture], shallow falloff on [ВТОРОСТЕПЕННОЕ].
[ЦВЕТ: Cool neutral colour grade / Warm tones against a neutral grade].
Commercial catalogue photography, 100mm macro, f/8.
[КАДР: 4:5 portrait], object fills about 70 percent of frame height, centred with generous margin.
No readable branding, no vignette, no shadow plate, no reflection puddle, no props, no hands, no text overlay, no watermark.
```

## Если результат «уехал» — дописать в конец

| Проблема | Добавить |
|---|---|
| Предмет мелкий | `tight crop, object fills 80 percent of frame height` |
| Серый или градиентный фон | `pure flat solid #0A0D14 background, no gradient, no backdrop, no floor` |
| Фальшивый логотип / текст | `completely blank surfaces, no lettering anywhere` |
| Появилась рука или модель | `product only, isolated object, no model, no hand, no skin` |
| Тяжёлая тень | `no shadow, no contact shadow, floating on flat background` |
| Слишком жёлтый | `neutral white balance, 5600K, no warm cast` |

## Правила серии
- Все фото каталога — **в одной сессии, одной моделью**, одним шаблоном: на сайте карточки стоят рядом, разный свет сразу виден.
- Выбилось одно фото — переделать **его**, тем же промптом, не меняя стиль всей серии.
- **Не писать реальную марку и модель** в промпте: получится чужой продукт, который нельзя публиковать.
  Для клиента — фото его реального товара как референс (`Use the uploaded image as the exact reference…`).
- Фон фото = фон сайта (или вырезать фон), чтобы товар «стоял» прямо на странице.
