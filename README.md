# zf2 album with doctrine2 ORM

This is a simple module from zf2 doc tutorial with doctrine2 ORM

Install
clone the module to your application

add new file named doctrine.local.php to config\autoload if not exists, (config\autoload\doctrine.local.php)

add this :

<?php

return array(
  'doctrine' => array(
    'connection' => array(
      'orm_default' => array(
        'driverClass' =>'Doctrine\DBAL\Driver\PDOMySql\Driver',
        'params' => array(
          'host'     => 'localhost',
          'port'     => '3306',
          'user'     => 'your-username',
          'password' => 'your_password',
          'dbname'   => 'your_database',
)))));

add this key 'Album' to application.config.php.
