# CodeIgniter - Blade Template Engine

### Installation

**Step 1:**

-> Download **blade** folder and past into **third_party** folder;

-> Download **blade.php** file and past into **libraries** folder;


**Step 2:** 

-> Go to **config** folder inside **autoload.php** add below code:

```php
require APPPATH.'/third_party/blade/Autoloader.php';
template\Blade\Autoloader::register();

```
**Step 3:**

-> And inside **autoload.php** add blade library: **$autoload['libraries'] = array('blade');**


**Step 4:**

-> Create folder **views** inside folder **cache**


### Usage 

- With data
```php
$data['message'] = "Hello!";
$this->blade->view('welcome_message', $data);
```
 - Without data
 ```php
 $this->blade->view('welcome_message');
 ```
------
You can't:

- use `@inject` `@can` `@cannot` `@lang` in a template file
- add any events or middleawares

Thanks for Laravel and it authors.

Documentation: [http://laravel.com/docs/5.4/blade](http://laravel.com/docs/5.3/blade)

Reference: https://github.com/XiaoLer/blade
