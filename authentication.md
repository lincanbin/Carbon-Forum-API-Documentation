# API Authentication Parameters

### Preparation
You need to set up a pair of correspondence and Key and Secret in ```config.php``` like this:
```php
<?php
/*
………………………………………………………………………………………………………………………………………………………………
………………………………………………………………………………………………………………………………………………………………
…………………………………………………………Other code…………………………………………………………………………
………………………………………………………………………………………………………………………………………………………………
………………………………………………………………………………………………………………………………………………………………
*/
// API checking data
// List<Map<String APIKey, String APISecret>>
// Free to modify
$APISignature = array();
$APISignature[12450] = 'b40484df0ad979d8ba7708d24c301c38';//For Android
```

###  Parameters
Key|Value Type|Description|Obligatory|Example
---|---|---|---|---
SKey|Integer|SKey=APIKey, you can find APIKey and APISecret in ```config.php```|√|12450
STime|Integer(10)|Unix Timestamp|√|1447253145
SValue|String(32)|md5(SKey:APISecret:STime)|×|89809a5201b04c608ffa50d63892a2ca

* md5("12450" + "b40484df0ad979d8ba7708d24c301c38" + "1447253145") = "89809a5201b04c608ffa50d63892a2ca"
