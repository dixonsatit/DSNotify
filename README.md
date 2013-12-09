DSNotify
========

Yii Notification extension

## Resources 
(noty) http://needim.github.io/noty/#theme

## Installation

* Extract the release file under `protected/extensions`
* In your `protected/config/main.php`, add the following:

```php
.....

'preload' => array('log','noty'),

....
'components' => array(
  ....
        'noty' => array(
            'class' => 'ext.dsnotify.DsNotify',
            //'layout'=>'topRight',
            //'theme'=>'default'
        ),
  ....
        ),
;;;

