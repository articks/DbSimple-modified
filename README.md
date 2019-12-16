# DbSimple-modified
DbSimple with mysqli support

```php
if(version_compare(phpversion(),"5.3.0",">=")) {
    require_once PATH_TO_DBSIMPLE."/Mysqli.php";
}
else {
    require_once PATH_TO_DBSIMPLE."/Mysql.php";
}
$db = DbSimple_Generic::connect("mysql://USER:PASSWORD@HOST/BASE");
$db->query("SET character_set_client = 'utf8', character_set_connection = 'utf8',character_set_results = 'utf8'");
```
