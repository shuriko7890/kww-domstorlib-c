# kww-domstorlib-c
## Using
First creates domstor builder:
```php
$builder = new Domstor_Builder();
```
Then build `$domstor` object, you must define two parameters `org_id` and `location_id`:

```php
$domstor = $builder->build(array(
    'org_id' => 3063,          // Organisation id
    'location_id' => 2653,  // Location id
));
```

Get `$list` object. You must specify `$page` number by getting it through request or some other way
```php
$list = $domstor->getList($object, $action, $page);
```
