## Multiple Authentication In Laravel 5.6

You can install Laravel 5.6 with Multiple Authentication (Admin and Users).

How to use:
1. Clone this repository
2. Run `composer install`
3. Rename .env.example to .env
4. Open .env file and setup your database
5. Run `php artisan key:generate`
6. Run `php artisan migrate`
7. Use tinker to set Admin email and password
      ```
      php artisan tinker
      $admin = App\Admin
      $admin->email = 'admin@app.com'
      $admin->password = Hash::make('adminpassword')
      $admin->save()
      
      ```
8. Run `php artisan serve` and go to localhost
