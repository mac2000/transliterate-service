Transliterate Service
=====================

This is simples ever service to transliterate text, I made it just to save my time in future scripts where I may need transliteration.

Transliterate API
-----------------

Transliteration service api is available via `http://transliterate-service.appspot.com/transliterate.(json|xml|txt)?q=Привет мир!`.

If you want to transliterate more that one string just provide as many `q` params as you need.

If you using it from javascript `callback` param is available for you.

Examples
--------

http://transliterate-service.appspot.com/transliterate.json?q=Привет мир!

    ["Privet mir!"]

http://transliterate-service.appspot.com/transliterate.json?q=Привет&q=Мир

    ["Privet", "Mir"]

http://transliterate-service.appspot.com/transliterate.json?q=Привет мир!&callback=transliterate

    transliterate(["Privet mir!"])

http://transliterate-service.appspot.com/transliterate.xml?q=Привет мир!

    <?xml version="1.0" encoding="utf-8"?>
    <items>
        <item>Privet mir!</item>
    </items>

http://transliterate-service.appspot.com/transliterate.txt?q=Привет мир!

    Privet mir!
