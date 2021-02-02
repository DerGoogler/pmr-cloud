# Debug Hybrid TTS!
Danger!

## AES Encode and Decode
Encode
```javascript
Android.AESencode('GG'); // XoFrpRkjgoKEw8ojYSnwPA==
```

Decode
```javascript
Android.AESdecode('XoFrpRkjgoKEw8ojYSnwPA=='); // GG
```

## Read File Path
Example
```javascript
var path = Android.getLocalFile('/sdcard/_DGS-DATA/Hybrid-TTS/debug/debug.tst');
// file content is default null
if (path === true) {
    console.log('debug access');
} else {
    console.log('No debug access');
}
```

## Androids SharedPrefs
Set or change a value
```javascript
var key = 'postkey';
var value = 4556; // You can use bools and strings too
Android.setCookie(key, value);
```

Get SharedPref
```javascript
var key = 'postkey';
Android.getCookie(key); // returns 4556
```

## Toast
Make an toast
```javascript
Android.Toast('I\'m an toast!');
```

## Play the TTS Voice
```javascript
Android.TTS_INPUT('Hello World!');
```

## Pitch and Speech
Set Pitch
```javascript
Android.pitch('0.1f');
Android.pitch('0.5f');
Android.pitch('1.0f');
```

Set Speech
```javascript
Android.speech('0.1f');
Android.speech('0.5f');
Android.speech('1.0f');
```

## Make Random String
```javascript
Android.makeRandomLetter('10');
// returns XXXXXXXXXX in upper case or lower case, it's random with numbers
```

## Close App
```javascript
Android.close();
```