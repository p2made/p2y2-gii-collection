yii2-p2y2-gii-collection v0.0.4
===============================

# Installation

Add...

```
	"p2made/yii2-p2y2-gii-collection": "dev-master"
```

to the `require-dev` section of your `composer.json` file & p2y2-things will be installed next time you run `composer update`.

## Usage


### claudejanz/yii2-mygii

```php
	//Add this into common/config/main-local.php
	'bootstrap' => 'gii',
	'modules' => [
		'gii' => [
			'class' => 'yii\gii\Module',
			'generators' => [
				'doubleModel' => [ // claudejanz/yii2-mygii
					'class' => 'claudejanz\mygii\generators\model\Generator',
				],
			],
		],
	],
```

### conquer/gii-modal

```php
	//Add this into common/config/main-local.php
	'bootstrap' => 'gii',
	'modules' => [
		'gii' => [
			'class' => 'yii\gii\Module',
			'allowedIPs' => ['127.0.0.1', '::1'],
			'generators' => [
				'modal_crud' => [ // conquer/gii-modal
					'class' => 'conquer\gii\templates\crud\Generator', // generator class
				]
			],
		],
	],
```

### deesoft/yii2-gii

```php
	//Add this into common/config/main-local.php
	'bootstrap' => 'gii',
	'modules' => [
		'gii' => [
			'class' => 'yii\gii\Module',
			'generators' => [
				'crud' => [ //deesoft/yii2-gii
					'class' => 'dee\gii\generators\crud\Generator'
				],
				'angular' => [ //deesoft/yii2-gii
					'class' => 'dee\gii\generators\angular\Generator'
				],
				'mvc' => [ //deesoft/yii2-gii
					'class' => 'dee\gii\generators\mvc\Generator'
				],
				'migration' => [ //deesoft/yii2-gii
					'class' => 'dee\gii\generators\migration\Generator'
				],
			],
		],
	],
```







### yii2mod/yii2-gii-extended


```php
	//Add this into common/config/main-local.php
	'bootstrap' => 'gii',
	'modules' => [
		'gii' => [
			'class' => 'yii\gii\Module',
			'generators' => [
				'enumerable' => [ //yii2mod/yii2-gii-extended
					'class' => 'yii2mod\gii\enum\Generator',
				],
				'crud' => [ //yii2mod/yii2-gii-extended
					'class' => 'yii2mod\gii\crud\Generator',
				],
			],
		],
	],
```



