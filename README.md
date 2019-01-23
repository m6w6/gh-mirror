# gh-mirror

Simple PHP webhook to mirror github repositories.

## Requirements

* [pecl/http](https://github.com/m6w6/ext-http)

## Configuration

```php
$mirror = getenv("mirror") ?: "/var/github/mirror";
$secret = getenv("secret") ?: trim(file_get_contents("$mirror/.secret"));
$owners = explode(",", getenv("owners") ?: trim(file_get_contents("$mirror/.owners")));
```

## License

gh-mirror is licensed under the 2-Clause-BSD license, which can be found in
the accompanying [LICENSE](./LICENSE) file.

## Contributing

All forms of contribution are welcome! Please see the bundled
[CONTRIBUTING](./CONTRIBUTING.md) note for the general principles followed.

The list of past and current contributors is maintained in [THANKS](./THANKS).
