# Auth Optional Laravel Api

This package will provide to login as user or login as a guest, so we will describe the package


## Usage

### In Kernel.php (app/Http/Kernel.php)
```php
    protected $routeMiddleware = [
        'auth.optional' => \App\Http\Middleware\AuthOptional::class
    ];
```

### In api.php
```php
Route::get('test', [TestController::class, 'index'])->middleware('auth.optional:api');
```
