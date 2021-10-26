# laravel8-cheat-sheet

//Creating laravel project with latest version
Composer create-project laravel/laravel projectname --prefer-dist

//Creating laravel project with specific version
Composer create-project laravel/laravel=8.0 projectname --prefer-dist



//PHP ARTISAN MIGRATIONS
//for creating a table through migration
php artisan make:migration create_projects_table --create=projects //create_tablename_table


//Table fields example with some important functionalities
$table->id();
$table->string('name', 55)->nullable();
$table->string('introduction', 500)->nullable();
$table->string('location', 55)->nullable();
$table->string('cost', 22)->default(0.00);
$table->string('created_at')->useCurrent();
$table->string('updated_at')->nullable();


//cach cleaning
php artisan view:clear
php artisan optimize
php artisan config:clear
php artisan config:cache

//for searching specific code/function from the project
clt + t 
