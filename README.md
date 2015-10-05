Simple class for build table ascii style.
Example:
```
<?php 
require_once('ClassBuildTableAascii.php'); 

$data = array (
 array (
 'Color' => 'Green',
 'Test' => 'Green',
 'Name' => 'Trixie',
 'Element' => 'Earth',
 'Likes' => 'Flowers'),
 array (
 'Name' => 'Tinkerbell',
  'Test' => 'Green',
 'Element' => 'Air',
 'Likes' => 'Singning',
 'Color' => 'Blue'),
 array (
 'Name' => 'Blum',
  'Test' => 'Green',
 'Element' => 'Water',
 'Likes' => 'Dancing',
 'Name' => 'Blum',
 'Color' => 'Pink')
);

/*
	public $newLineDelimiter = "<br>";
	public $topBorderDelimiter = "-";
	public $sideDelimiter = "|";
	public $space = "&nbsp;";
	public $angle = "+";
*/
$table = new ClassBuildTableAascii($data);


echo $table->asHtml();
echo $table->asText();
?>
```