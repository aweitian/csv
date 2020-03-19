# 测试
```php```
require "csv.php";


$csv = new Csv();
$cv = array(
  "ID",
  "编号",
  "姓名",
  "cc",
);



$dl_data = array($cv);

$dl_data[] = array(
      111,
      "30852695748569854",
      "张三行",
      "adf",
  );
$dl_data[] = array(
      22,
      "30852695748569852",
      "大型",
      "dsds",
  );
$date = date("Y-m-d");
$csv->downloadCsvData($dl_data, "数据({$date}).csv");
```