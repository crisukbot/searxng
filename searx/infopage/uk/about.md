# Про SearXNG

SearXNG це [метапошукова система], яка агрегує результати інших
{{link('пошукових рушіїв', 'preferences')}} не зберігаючи при цьому інформацію 
про своїх користувачів.

Проект SearXNG керується відкритою спільнотою, якщо у вас є питання,
або ви просто хочете поспілкуватись, приєднуйтесь до нас в Matrix [#searxng:matrix.org]

Зробимо SearXNG краще.

- Ви можете покращити переклад SearXNG на [Weblate] або...
- Відстежувати розвиток, надсилати внески та повідомляти про проблеми на [SearXNG sources].
- Щоб отримати додаткову інформацію, відвідайте проектну документацію SearXNG за адресою [SearXNG
  docs].

## Навіщо його використовувати?

- SearXNG може не пропонувати вам настільки персоналізовані результати, як Google, але він не
  не створює профіль про вас.
- SearXNG не цікавиться тим, що ви шукаєте, ніколи не ділиться інформацією з
  третьою стороною і не може бути використаний проти вас.
- SearXNG - це вільне програмне забезпечення, код на 100% відкритий, і кожен може
  зробити його кращим.

Якщо ви дбаєте про конфіденційність, хочете бути свідомим користувачем або іншим чином вірите
в цифрову свободу, зробіть SearXNG пошуковою системою за замовчуванням або запустіть її на своєму
власному сервері!

## Як зробити його пошуковою системою за замовчуванням?

SearXNG підтримує [OpenSearch].  Для отримання додаткової інформації про зміну пошукової системи за замовчуванням
дивіться документацію до вашого браузера:

- [Firefox]
- [Microsoft Edge] - За посиланням ви також знайдете кілька корисних інструкцій
  для Chrome та Safari.
- [Chromium]-based браузери додають лише ті сайти, на які користувач переходить без
  шляху.

При додаванні пошукової системи не повинно бути дублікатів з однаковою назвою.  Якщо
ви зіткнулися з проблемою, і не можете додати пошукову систему, ви можете

- видалити дублікат (назва за замовчуванням: SearXNG) або
- зв'язатися з власником інстансу, щоб дати йому іншу назву, ніж за замовчуванням.

## Як це працює?

SearXNG - це форк відомого [searx] [метапошукової системи], який був
натхненний проектом [Seeks].  Він забезпечує базову конфіденційність, змішуючи ваші
запити з пошуком на інших платформах без збереження даних пошуку.  SearXNG
можна додати в пошуковий рядок вашого браузера; крім того, його можна встановити як
пошуковою системою за замовчуванням.

Сторінка {{link('статистики', 'stats')}}  містить деяку корисну анонімну 
статистику про використані рушії.

## Як я можу запустити свій інстанс SearXNG?

SearXNG цінує вашу стурбованість щодо логів, тому візьміть код з
[SearXNG sources] і запустіть його самостійно!

Додайте свій інстанс до цього [списку публічних
інстансів]({{get_setting('brand.public_instances')}}), щоб допомогти іншим людям
відновити свою приватність і зробити інтернет вільнішим.  Чим більш децентралізованим є
інтернет, тим більше свободи ми маємо!

[SearXNG sources]: {{GIT_URL}}
[#searxng:matrix.org]: https://matrix.to/#/#searxng:matrix.org
[SearXNG docs]: {{get_setting('brand.docs_url')}}
[searx]: https://github.com/searx/searx
[метапошукова система]: https://uk.wikipedia.org/wiki/%D0%9C%D0%B5%D1%82%D0%B0%D0%BF%D0%BE%D1%88%D1%83%D0%BA%D0%BE%D0%B2%D0%B0_%D1%81%D0%B8%D1%81%D1%82%D0%B5%D0%BC%D0%B0
[метапошукової системи]: https://uk.wikipedia.org/wiki/%D0%9C%D0%B5%D1%82%D0%B0%D0%BF%D0%BE%D1%88%D1%83%D0%BA%D0%BE%D0%B2%D0%B0_%D1%81%D0%B8%D1%81%D1%82%D0%B5%D0%BC%D0%B0
[Weblate]: https://translate.codeberg.org/projects/searxng/
[Seeks project]: https://beniz.github.io/seeks/
[OpenSearch]: https://github.com/dewitt/opensearch/blob/master/opensearch-1-1-draft-6.md
[Firefox]: https://support.mozilla.org/uk/kb/dodati-abo-vidaliti-poshukovi-sistemi-v-firefox
[Microsoft Edge]: https://support.microsoft.com/uk-ua/microsoft-edge/%D0%B7%D0%BC%D1%96%D0%BD%D0%B8%D1%82%D0%B8-%D0%B7%D0%B0%D1%81%D1%96%D0%B1-%D0%BF%D0%BE%D1%88%D1%83%D0%BA%D1%83-%D0%B7%D0%B0-%D0%B7%D0%B0%D0%BC%D0%BE%D0%B2%D1%87%D1%83%D0%B2%D0%B0%D0%BD%D0%BD%D1%8F%D0%BC-f863c519-5994-a8ed-6859-00fbc123b782
[Chromium]: https://www.chromium.org/tab-to-search
