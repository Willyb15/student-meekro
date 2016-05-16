###Practice PHP with mySQL and Meekro
###Wrote a few arrays with PHP
```php
$students = array('student'=>'Tristan', 'Josh', 'Bogdan', 'student2'=>'Lazlo', 'Keith', 'Will', 'Curtis', 'Joe', 'Kochan', 'Patrick', 'Jonathan', 'Jeremy');

$students1 = array(
	'Tristan', 
	'Josh', 
	'Bogdan', 
	'Lazlo', 
	'Keith', 
	'Will', 
	'Curtis', 
	'Joe', 
	'Kochan', 
	'Patrick', 
	'Jonathan', 
	'Jeremy'
);
$students2 = array(
	'student0' => 'Tristan', 
	'student1' => 'Josh', 
	'student2' => 'Bogdan', 
	'student3' => 'Lazlo', 
	'student4' => 'Keith', 
	'student5' => 'Will', 
	'student6' => 'Curtis', 
	'student7' => 'Joe', 
	'student8' => 'Kochan', 
	'student9' => 'Patrick', 
	'student10' => 'Jonathan', 
	'student11' => 'Jeremy'
);
print "<pre>";
print_r($students2);
print "</pre>";
```
###Connected to mySQL DB
```php
	
	$link = mysql_connect('127.0.0.1', 'x', 'x');
	if(!$link){
		print 'not connected' . mysql_error();
		exit;
	}
	$db_selected = mysql_select_db('phpsandbox', $link);
	if(!$db_selected){
		die("Cannot use database phpsandbox:" . mysql_error());
	}
	```
	###Dowloaded Meekro (meekrodb.2.3.class.php) and put in Directory
	###Connected to Meekro DB
	```php
	require_once 'meekrodb.2.3.class.php';
DB::$user = 'x';
DB::$password = 'x';
DB::$dbName = 'phpsandbox';
DB::$host = '127.0.0.1';
```
