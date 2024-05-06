# MonMaZa.io

Projects
https://poslite.marketplace.com.mm
https://npc.zacompany.dev (for https://netpachi.com)

https://vue3datepicker.com/props/keyboard/

https://animate.style/

https://medium.com/front-end-weekly/build-a-css-only-toggle-switch-using-tailwindcss-d2739882934

# Laravel

- # Specific migration table file running
- php artisan migrate --path=/database/migrations/your_migration_table.php



# Ebooks
- # Design Patterns
- https://designpatterns.saturngod.net/?fbclid=IwAR1cfV-vliUf8z2bytEqGRxZ0vCFXoZgbZeuo4FPE_LYhcM9K4aSYrKXWM0

# MySQl

Installation process:
1. Now simply run the below command in your terminal

$ brew install mysql
2. Start the MySQL service

$ brew services start mysql
3. Set root MySQL password

$ mysqladmin -u root password 'secretpassword'
4. Access MySQL on mac

$ mysql -u root -p
Command will ask the password you just set in the previous step.

ALSO READ
7 TV Shows Every Programmer Should Binge Watch
7 TV Shows Every Programmer Should Binge Watch
 

Things to remember
Stop MySQL service on Mac start

If you don't want MySQL service to start every time you start your mac then run the below command

$ brew services stop mysql
This will stop the MySQL service from running in the background.

Start MySQL service

You can always run the below command to start the MySQL server on mac and it will not start on the next computer restart

$ mysql.server start
Stop MySQL service

If you want to immediately stop the MySQL service then run the below command

$ mysql.server stop
GUI clients to access database

And you can also access your database with mac MySQL client to make your life easy. Here are a couple of suggestions:

Sequel Pro - https://www.sequelpro.com/
TablePlus - https://tableplus.com/

# Produce ER Diagram from Laravel
You can install Laravel ER Diagram Generator via Composer by running:
lua
- composer require beyondcode/laravel-er-diagram-generator --dev

- brew install graphviz

- php artisan generate:erd

# Folding in VS code
Fold folds the innermost uncollapsed region at the cursor:

Ctrl + Shift + [ on Windows and Linux
⌥ + ⌘ + [ on macOS
Unfold unfolds the collapsed region at the cursor:

Ctrl + Shift + ] on Windows and Linux
⌥ + ⌘ + ] on macOS
Fold All folds all regions in the editor:

Ctrl + K, Ctrl + 0 (zero) on Windows and Linux
⌘ + K, ⌘ +0 (zero) on macOS
Unfold All unfolds all regions in the editor:

Ctrl + K, Ctrl + J on Windows and Linux
⌘ + K, ⌘ + J on macOS

# VS Code Tip & Tricks
https://github.com/Microsoft/vscode-tips-and-tricks#find-all-references

# Laravel Jenssenger Agent to access http header user-agent
https://github.com/jenssegers/agent

# GitHub
- git add  ***/***/***/ProductController.php
- git status
- git commit -m "*****"
- git pull origin main
- git config pull.rebase false
- git branch
- git checkout *** (change branch)
- git push origin main
- Merge(Commit on left pane on vs code)
- git log --oneline (check log)

# Add a column on the production database
- php artisan make:migration add_column_name_to_table_name --table=table_name
- <?php

use Illuminate\Database\Migrations\Migration;
use Illuminate\Database\Schema\Blueprint;
use Illuminate\Support\Facades\Schema;

class AddColumnNameToTableName extends Migration
{
    public function up()
    {
        Schema::table('table_name', function (Blueprint $table) {
            $table->string('column_name')->nullable(); // Change data type as needed
        });
    }

    public function down()
    {
        Schema::table('table_name', function (Blueprint $table) {
            $table->dropColumn('column_name');
        });
    }
}
- php artisan migrate

# Make a backup of production database
- ssh your_username@your_server_ip
- cd /var/backups [anyPath]
- pg_dump -U your_username -d your_database_name -f your_backup_file_name.sql [pg_dump is for PostgresSQL]
- secure the backup file [chmod 600 your_backup_file_name.sql]
- scp your_username@your_server_ip:/var/backups/your_backup_file_name.sql /path/to/local/directory [download file]

# Database Backup in Laravel
- composer require spatie/laravel-backup
- php artisan vendor:publish --provider="Spatie\Backup\BackupServiceProvider"
- php artisan backup:run
- app/Console/Kernel.php -> protected function schedule(Schedule $schedule)
{
    $schedule->command('backup:run')->daily()->at('01:00');

}

# Map/Through 
https://zadeveloper.slack.com/archives/D066JQ8A5QD/p1712817394326999

#instead of var_export ( php array())
https://github.com/brick/varexporter

# ICons
https://icones.js.org/





