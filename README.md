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
```

## Usage

### PHP
```php
Yii::app()->noty->noty('message', 'warning', 'top');

Yii::app()->noty->noty('message', 'alert', 'topLeft');
Yii::app()->noty->noty('message', 'error', 'topCenter');
Yii::app()->noty->noty('message', 'success', 'topRight');

Yii::app()->noty->noty('message', 'infomation', 'centerLeft');
Yii::app()->noty->noty('message', 'alert', 'center');
Yii::app()->noty->noty('message', 'alert', 'centerRight');

Yii::app()->noty->noty('message', 'alert', 'bottomLeft');
Yii::app()->noty->noty('message', 'alert', 'bottomCenter');
Yii::app()->noty->noty('message', 'alert', 'bottomRight');
Yii::app()->noty->noty('message', 'error', 'bottom');
```

### Javascript
```js
 var n = noty({
            text: 'message',
            type: 'success',
            timeout: 3000,
            dismissQueue: true,
            layout: 'center',
            theme: 'defaultTheme'
        });
```





