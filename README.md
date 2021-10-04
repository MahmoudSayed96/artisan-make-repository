# artisan-make-repository
Code for php artisan command make repository directory.

## Setup Steps:
- Add `MakeRepositoryCommand.php` file in this path `app/Console/Commands`
- Add `stubs` folder in this path `app/Console/Commands`
- Go to `Kernel.php` in path `` and add this code
```php
 /**
   * The Artisan commands provided by your application.
   *
   * @var array
  */
    protected $commands = [
        MakeRepositoryCommand::class,
    ];
```
- Add `Repositories` folder in this path `app`
 > This folder contains the `BaseRepository.php` file you can change code in this file for suitable with you.

## Command for generate repository class
```bash
  php artisan make:repository UserRepository
```
