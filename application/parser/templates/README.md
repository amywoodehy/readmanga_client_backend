# Regular Expression template
 for parsing grouple.ru websites

* should return list of manga-pages (images) in strict numeration

```javascript
[
    'some.cdn.net/image1.png',
    'some.cdn.net/image2.png',
    'some.cdn.net/image3.png',
    ...
    'some.cdn.net/imageN.png',
]
```
* should return list of dicts containing commentaries

```javascript
[
    {
        'page': 1,
        'comments': [
            {
                'username': 'Ololowka32',
                'date': DateTime,
                'comm': 'Mamku watal',
            },
            {
                'username': 'SomeSerious',
                'date': DateTime,
                'comm': 'That was funny',
            },
            {
                'username': 'Wtfdude',
                'date': DateTime(),
                'comm': 'that plot twist...',
            }
        ]
    },
    {
        'page': 2,
        'comments': [],
    },
]
```
* and return list of manga. easiest thing

```javascript
[
    {
        'manga_name': 'Boruto',
        'url': 'some.url.net/boruto',
        'cover': 'some.url.net/borutocover.png',
        'genre': 'action, comedy, someshit',
        'number_of_chapters': 999,
        'stars': 9.99,
    }
]
```

* list of chapters of given manga

```javascript
[
    {
        'volume': 1
        'chapter': 1
        'name': 'Raise of new hope',
        'url': 'example.com/boruto/vol1/1',
    }
]
```