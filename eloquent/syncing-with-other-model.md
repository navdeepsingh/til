# Syncing with other model

With sync method we can easily add/sync data to the DB
```php
$user->roles()->sync([1, 2, 3]);
```
sync() will keep in DB the IDs you pass to it
