# Syncing with other model

With sync method we can easily add/sync data to the DB
```php
$user->roles()->sync([1, 2, 3]);
```
sync() will keep in DB the IDs you pass to it, other will delete from DB automatically.

And in attach() and detach() we can add role and remove role apparently from DB one by one.

