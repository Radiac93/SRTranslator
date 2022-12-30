# DeepL translator

## Usage

Driver is optional, if not passed as argument the code will create a new firefox driver with geckodriver (and yes, it install it and put in path if needed) and setup free proxies to avoid getting banned

```
from srtranslator.translators.deepl import DeeplTranslator

translator = DeeplTranslator(driver=driver)

translator.translate(text, source_language, destination_language)

translator.quit()
```

## Supported languages

```
auto : Any language (detect)
bg : Bulgarian
zh : Chinese
cs : Czech
da : Danish
nl : Dutch
en : English
et : Estonian
fi : Finnish
fr : French
de : German
el : Greek
hu : Hungarian
it : Italian
ja : Japanese
lv : Latvian
lt : Lithuanian
pl : Polish
pt : Portuguese
ro : Romanian
ru : Russian
sk : Slovak
sl : Slovenian
es : Spanish
sv : Swedish
```

## Limitations

DeepL won't let you translate more than 3000 characters at the same time.