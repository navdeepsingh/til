# Get both models fields including pivot table

Using with on parent model
```php
$user = App\User::with('roles')->first();
```

