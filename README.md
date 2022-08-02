# google-translate


Require module and pass in your API Google project API key after enabling the API service. Note: This module currently doesn't support oauth authentication.
```
var googleTranslate = require('google-translate')(apiKey, options);
```
### String translation:
```
googleTranslate.translate('My name is Brandon', 'es', function(err, translation) {
  console.log(translation.translatedText);
  // =>  Mi nombre es Brandon
});
```
### Language detection:
```
googleTranslate.detectLanguage('Gracias', function(err, detection) {
  console.log(detection.language);
  // =>  es
});
```
