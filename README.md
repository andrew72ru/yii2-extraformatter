# yii2-extraformatter
Additional functions to Yii2 formatter

* Place this file to your `common/modules/formatter` direcory (create it, if not exists) or somwhere else
* Edit a `namespace` description in `FormatterExt.php`
* Set code of your city in `FormatterExt.php`
* Create a config like the following:

``` php
'components' => [
  …
  'formatter' => [
    'class' => 'common\modules\formatter\FormatterExt',
    …
  ]
]
```

* Use :)

### Example

`echo Yii::$app->Formatter->asPhone(79617815451)` displays +7 (961) 781-54-51

`echo Yii::$app->Formatter->asPhone(273700)` displays +7 (3452) 27-37-00

`echo Yii::$app->Formatter->asSpellMoney(25383.60)` displays «Двадцать пять тысяч триста восемьдесят три рубля 60 копеек»
