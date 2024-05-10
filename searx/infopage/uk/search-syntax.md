# Синтаксис пошуку

SearXNG містить синтаксис пошуку, за допомогою якого ви можете змінювати категорії,
рушії, мови та інше.  Перейдіть до {{link('preferences', 'preferences')}} для отримання
списку рушіїв, категорій і мов.

## `!` вибір рушія та категорії

Щоб задати назву категорії та/або рушія, використовуйте префікс `!`.  Наведемо кілька прикладів:

- пошук у Вікіпедії **Київ**

  - {{search('!wp Київ')}}
  - {{search('!wikipedia Київ')}}

- пошук в категорії **мапа** для **Київ**

  - {{search('!map Київ')}}

- пошук зображення

  - {{search('!images Wau Holland')}}

Скорочення рушіїв та мов також приймаються.  Модифікатори рушіїв/категорій
можуть бути ланцюжковими та інклюзивними.  Наприклад, за допомогою {{search('!map !ddg !wp
Київ')}} працює пошук відразу і в категорії мапи, а також у DuckDuckGo та Вікіпедії - **Київ**.

## `:` вибрати мову

Для увімкнення мовного фільтра використовуйте префікс `:`.  Наведемо приклад:

- пошук у Вікіпедії користувацькою мовою

  - {{search(':fr !wp Wau Holland')}}

## `!!<bang>` зовнішній чубчик

SearXNG supports the external bangs from [DuckDuckGo].  To directly jump to a
external search page use the `!!` prefix.  To give an example:

- search Wikipedia by a custom language

  - {{search('!!wfr Wau Holland')}}

Please note, your search will be performed directly in the external search
engine, SearXNG cannot protect your privacy on this.

[DuckDuckGo]: https://duckduckgo.com/bang

## `!!` automatic redirect

When mentioning `!!` within the search query (separated by spaces), you will
automatically be redirected to the first result.  This behavior is comparable to
the "Feeling Lucky" feature from DuckDuckGo.  To give an example:

- search for a query and get redirected to the first result

  - {{search('!! Wau Holland')}}

Please keep in mind that the result you are being redirected to can't become
verified for being trustworthy, SearXNG cannot protect your personal privacy
when using this feature.  Use it at your own risk.

## Special Queries

In the {{link('preferences', 'preferences')}} page you find keywords for
_special queries_.  To give a few examples:

- generate a random UUID

  - {{search('random uuid')}}

- find the average

  - {{search('avg 123 548 2.04 24.2')}}

- show _user agent_ of your browser (needs to be activated)

  - {{search('user-agent')}}

- convert strings to different hash digests (needs to be activated)

  - {{search('md5 lorem ipsum')}}
  - {{search('sha512 lorem ipsum')}}
