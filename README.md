#
Skimbug is a browser extension that reads web pages for you. It shows what the page is about, retells the part you are looking at, picks the links worth opening, blocks ads, and sends a little electronic bug crawling over the text to mark the important words.

Everything except the summary works on your computer, for free, without any account. The summary uses an AI model you connect yourself; free ones are enough.


## 1. Install

You need Chrome, or any browser built on it: Edge, Brave, Arc, Opera, Yandex Browser.

1. **Unzip** the archive. Put the `skimbug` folder somewhere it can stay for good, for example in Documents. The browser runs the extension straight from this folder, so don't delete or move it later.
2. Open a new tab and type `chrome://extensions` in the address bar. In Edge it's `edge://extensions`, in Yandex Browser `browser://extensions`.
3. Switch on **Developer mode**. The switch is in the top right corner (in Edge, on the left).
4. Press **Load unpacked** and pick the `skimbug` folder: the one that has `manifest.json` directly inside it.
5. Skimbug appears in the list. Click the puzzle-piece icon next to the address bar and pin Skimbug so its icon is always visible.
6. **Reload the tabs you already had open**, otherwise Skimbug can't see them.

The browser may show a note that you're using developer-mode extensions. That's normal for extensions installed from a folder; close it.

## 2. First launch

Click the Skimbug icon or press **Alt + S**. A panel opens on the right side of the browser.

1. **Pick a language**: English or Russian. You can change it later in Settings.
2. A short **welcome guide** explains how it works. Step 3 has a box for your key (see below). You can skip it and connect later.

## 3. Turn on summaries: get a free key

A key is a long password that lets Skimbug use an AI model on your behalf. Getting one takes about two minutes and needs no bank card.

| Service | Where to get the key | Good to know |
|---|---|---|
| **Google Gemini** | [aistudio.google.com/apikey](https://aistudio.google.com/apikey) | The most generous free plan. Google doesn't offer it in every country. |
| **OpenRouter** | [openrouter.ai/keys](https://openrouter.ai/keys) | Many free models, about 50 requests a day. |
| **Groq** | [console.groq.com/keys](https://console.groq.com/keys) | Very fast, about 1,000 requests a day, but takes shorter texts. |

1. Open one of the links, sign in, press **Create key** (the wording differs a little between sites) and copy the key.
2. In Skimbug, open **Settings → Models** and paste it into **Paste any API key**.
3. Skimbug recognises whose key it is by its shape. Press **Connect**. Skimbug checks the key with the provider and picks a suitable model.

**Add a second key from a different service.** When the first one runs out of free requests or stops answering, Skimbug quietly asks the next one and shows a yellow note saying which model answered instead.

Already paying for **OpenAI, Anthropic, Mistral or DeepSeek**? Paste that key the same way. If you run models on your own computer with **Ollama**, open **More options** and choose Ollama; it needs no key.

## 4. Using it

### Top of the panel
The name of the page, how long it is, and a **page map**: a strip that shows where the article is (blue), side boxes (pink), clutter like menus and footers (grey) and ads (red). The white frame is the part on your screen right now. Click the strip to jump there. **Outline on page** draws these zones on the page itself.

### Overview
- **Summarize in English / in Russian.** Nothing is sent to the AI until you press one of them. The page's language doesn't matter: an English article can be retold in Russian and the other way round.
- **About this page**: two or three sentences on what it's about.
- **On your screen now**: a closer retelling of only what you see. When you scroll, a button appears to retell the new part.
- **Key links** and **Also on this page**: the links worth opening, each with a reason. **Show** scrolls the page to that link.
- The **model button** at the top of the box switches which model answers first.

Opening the same article again costs nothing: answers are saved for a week.

### Links
Every useful link on the page, sorted into links to other sites, links within this site, and links from side boxes. **Left out** shows how many menu, ad and repeat links were dropped. **Copy all links** copies them with their titles.

### Blocker
Ads and trackers are blocked on every site automatically, before they load. The big number shows how much was removed from the page.

- **Pause on this site**: for when a site breaks or refuses to work with a blocker. The page reloads with ads.
- **Show what was removed**: puts the hidden pieces back with a red outline, so you can see what was cut.
- **Clean page**: **Fade** dims everything except the article and the site's logo; **Hide** removes it all from view. **Off** brings the page back. Nothing is deleted, and it lasts until you reload.

### Settings
- **Language**: English or Russian interface.
- **Models**: your keys, in the order they are tried. Arrows change the order, **Remove** deletes a key from the browser.
- **Text sent per request**: leave it on **Auto**.
- **Never send text from**: sites whose text never leaves your browser. Your email, banks and government sites are there from the start. Add your own bank's address too. Pages with a password or card field are always skipped.
- **Crawlers**: pick the bug (centipede, beetle, spider, scorpion, or a random one on each page) and its colour. **By word type** colours the words it marks: nouns, verbs, adjectives and so on. **Follow my mouse** (also the cursor button at the top of the panel) makes the bug chase your cursor and mark every word it runs over.

## 5. Privacy

- Your keys are stored only in this browser on your computer and go only to the service they belong to. They are not in the extension's files and Skimbug has no server.
- Page text leaves your computer only when you press Summarize, and only to the model you connected.
- Skimbug collects no statistics and needs no account.
- **Never paste your key into a chat, an email or a screenshot.** If you think someone saw it, delete it on the service's site and create a new one.

## 6. If something doesn't work

| What you see | What to do |
|---|---|
| The panel says it can't read the page | Reload the page. Browser pages (`chrome://…`) and the extension store can't be read by any extension. |
| "is not available in your country" | That service doesn't work in your region. Connect another one, for example OpenRouter or Groq. |
| "rejected the key" | The key was copied with a missing piece or was deleted. Create a new one and paste it again. |
| "ran out of free requests" | The daily limit is used up. Add a second key from another service or wait; Skimbug shows when it will try again. |
| A site looks broken | Blocker → **Pause on this site**. |
| The bug gets in the way | Settings → turn off **Show a crawler on pages**. |
| Nothing happens after an update | `chrome://extensions` → press the round arrow on Skimbug's card, then reload your tabs. |

## 7. Updating and removing

**Update:** replace the contents of the `skimbug` folder with the new version, then press the round arrow on Skimbug's card in `chrome://extensions`. Your keys and settings stay.

**Remove:** `chrome://extensions` → **Remove** on Skimbug's card. This also deletes your keys and settings from the browser. Then you can delete the folder.

---

<a id="русский"></a>

# Skimbug

[English](#skimbug) · **Русский**

Skimbug — расширение для браузера, которое читает страницы за вас. Оно показывает, о чём страница, пересказывает то, что у вас на экране, выбирает ссылки, которые стоит открыть, блокирует рекламу и запускает по тексту маленького электронного жука, который отмечает важные слова.

Всё, кроме пересказа, работает на вашем компьютере, бесплатно и без аккаунта. Для пересказа нужна нейросеть, которую вы подключаете сами; бесплатных хватает.


## 1. Установка (2 минуты, права администратора не нужны)

Нужен Chrome или любой браузер на его основе: Edge, Brave, Arc, Opera, Яндекс Браузер.

1. **Распакуйте** архив. Положите папку `skimbug` туда, где она будет лежать постоянно, например в «Документы». Браузер запускает расширение прямо из этой папки, поэтому потом её нельзя удалять или переносить.
2. Откройте новую вкладку и введите в адресную строку `chrome://extensions`. В Edge — `edge://extensions`, в Яндекс Браузере — `browser://extensions`.
3. Включите **Режим разработчика** (Developer mode). Переключатель в правом верхнем углу (в Edge — слева).
4. Нажмите **Загрузить распакованное** (Load unpacked) и выберите папку `skimbug` — ту, внутри которой сразу лежит `manifest.json`.
5. Skimbug появится в списке. Нажмите на значок пазла рядом с адресной строкой и закрепите Skimbug, чтобы его иконка всегда была на виду.
6. **Перезагрузите уже открытые вкладки**, иначе Skimbug их не увидит.

Браузер может показать предупреждение о расширениях в режиме разработчика. Для расширений, установленных из папки, это нормально — просто закройте его.

## 2. Первый запуск

Нажмите на иконку Skimbug или **Alt + S**. Справа откроется панель.

1. **Выберите язык**: английский или русский. Потом его можно поменять в настройках.
2. Короткий **вводный гид** объяснит, как всё устроено. На третьем шаге есть поле для ключа (см. ниже). Можно пропустить и подключить позже.

## 3. Включите пересказ: получите бесплатный ключ

Ключ — это длинный пароль, по которому Skimbug обращается к нейросети от вашего имени. Получить его — минуты две, банковская карта не нужна.

| Сервис | Где взять ключ | Что важно знать |
|---|---|---|
| **Google Gemini** | [aistudio.google.com/apikey](https://aistudio.google.com/apikey) | Самый щедрый бесплатный тариф. Google открыл его не во всех странах. |
| **OpenRouter** | [openrouter.ai/keys](https://openrouter.ai/keys) | Много бесплатных моделей, около 50 запросов в день. |
| **Groq** | [console.groq.com/keys](https://console.groq.com/keys) | Очень быстрый, около 1000 запросов в день, но берёт тексты покороче. |

1. Откройте одну из ссылок, войдите, нажмите **Create key** (на разных сайтах кнопка называется чуть по-разному) и скопируйте ключ.
2. В Skimbug откройте **Настройки → Модели** и вставьте его в поле **Вставьте любой API-ключ**.
3. Skimbug сам поймёт по виду ключа, чей он. Нажмите **Подключить**. Skimbug проверит ключ у провайдера и выберет подходящую модель.

**Добавьте второй ключ от другого сервиса.** Когда у первого кончатся бесплатные запросы или он перестанет отвечать, Skimbug сам спросит следующий и покажет жёлтую плашку: какая модель ответила вместо первой.

Уже платите за **OpenAI, Anthropic, Mistral или DeepSeek**? Вставьте этот ключ так же. Если запускаете модели у себя на компьютере через **Ollama**, откройте **Ещё** и выберите Ollama — ключ не нужен.

## 4. Как пользоваться

### Верх панели
Название страницы, её длина и **карта страницы** — полоска, на которой видно, где статья (голубое), боковые блоки (розовое), лишнее вроде меню и подвала (серое) и реклама (красное). Белая рамка — то, что сейчас у вас на экране. Нажмите на полоску, чтобы перейти к этому месту. **Обвести на странице** рисует эти зоны прямо на сайте.

### Обзор
- **Пересказать на английском / на русском.** Пока вы не нажали одну из кнопок, в нейросеть ничего не уходит. Язык страницы не важен: английскую статью можно пересказать по-русски и наоборот.
- **О чём страница** — два-три предложения о сути.
- **Сейчас на экране** — подробный пересказ только того, что вы видите. Когда прокрутите, появится кнопка, чтобы пересказать новый кусок.
- **Главные ссылки** и **Ещё на странице** — ссылки, которые стоит открыть, с пояснением. **Показать** прокручивает страницу к ссылке.
- **Кнопка модели** сверху переключает, какая модель отвечает первой.

Повторное открытие той же статьи ничего не стоит: ответы хранятся неделю.

### Ссылки
Все полезные ссылки страницы, разложенные на ссылки на другие сайты, на этот сайт и из боковых блоков. **Отброшено** показывает, сколько ссылок из меню, рекламы и повторов выкинуто. **Скопировать все** копирует их вместе с названиями.

### Блокер
Реклама и трекеры блокируются на всех сайтах автоматически, ещё до загрузки. Большая цифра — сколько всего убрано со страницы.

- **Пауза на этом сайте** — если сайт сломался или не пускает с блокировщиком. Страница перезагрузится с рекламой.
- **Показать, что убрано** — возвращает скрытое с красной рамкой, чтобы было видно, что вырезано.
- **Чистая страница**: **Приглушить** — затемняет всё, кроме статьи и логотипа сайта; **Скрыть** — убирает это совсем. **Выкл** возвращает страницу как была. Ничего не удаляется, и всё сбрасывается после перезагрузки.

### Настройки
- **Язык** — интерфейс на английском или русском.
- **Модели** — ваши ключи в том порядке, в котором их пробуют. Стрелки меняют порядок, **Удалить** стирает ключ из браузера.
- **Сколько текста отправлять за запрос** — оставьте **Авто**.
- **Никогда не отправлять текст с** — сайты, текст которых никогда не покидает браузер. Почта, банки и госсайты там с самого начала. Добавьте адрес своего банка. Страницы с полем пароля или карты пропускаются всегда.
- **Краулеры** — выберите жука (многоножка, жук, паук, скорпион или случайный на каждой странице) и его цвет. **По части речи** раскрашивает отмеченные слова: существительные, глаголы, прилагательные и так далее. **Следовать за мышью** (то же — кнопка с курсором вверху панели) заставляет жука гоняться за курсором и отмечать все слова на пути.

## 5. Приватность

- Ключи хранятся только в этом браузере на вашем компьютере и уходят только тому сервису, которому принадлежат. В файлах расширения их нет, сервера у Skimbug нет.
- Текст страницы покидает компьютер, только когда вы нажимаете «Пересказать», и только в ту нейросеть, которую вы подключили.
- Skimbug не собирает статистику и не требует аккаунта.
- **Никогда не вставляйте ключ в чат, письмо или на скриншот.** Если думаете, что его кто-то видел, удалите его на сайте сервиса и создайте новый.

## 6. Если что-то не работает

| Что видите | Что делать |
|---|---|
| Панель пишет, что не может прочитать страницу | Перезагрузите страницу. Служебные страницы браузера (`chrome://…`) и магазин расширений не может читать ни одно расширение. |
| «не работает в вашей стране» | Этот сервис недоступен в вашем регионе. Подключите другой, например OpenRouter или Groq. |
| «ключ не принят» | Ключ скопирован не целиком или удалён. Создайте новый и вставьте заново. |
| «закончились бесплатные запросы» | Дневной лимит исчерпан. Добавьте второй ключ от другого сервиса или подождите — Skimbug покажет, когда попробует снова. |
| Сайт выглядит сломанным | Блокер → **Пауза на этом сайте**. |
| Жук мешает | Настройки → выключите **Показывать краулера на страницах**. |
| После обновления ничего не работает | `chrome://extensions` → круглая стрелка на карточке Skimbug, потом перезагрузите вкладки. |

## 7. Обновление и удаление

**Обновить:** замените содержимое папки `skimbug` новой версией и нажмите круглую стрелку на карточке Skimbug в `chrome://extensions`. Ключи и настройки сохранятся.

**Удалить:** `chrome://extensions` → **Удалить** на карточке Skimbug. Вместе с ним из браузера удалятся ключи и настройки. После этого папку можно стереть.
