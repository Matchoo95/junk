<!DOCTYPE html>

<html>
<head>
  <title>察しゲーム</title>

</head>

<body>

<center>
  <h1>察しゲーム</h1>

<?php

$guess = $_POST["guess"];
$number = $_POST["number"];


if(empty ($number) ) {
  print ("<h4>ようこそ！私は一つの番号を持っています、察してください！</h4><br />");
  $number = rand(1, 100);
} elseif ($number == $guess) {
    print ("<h4>おめでとうございます！正解です！あなたは $number を察しました！</h4><br />");
} elseif ($guess < $number) {
    print ("<h4>もっと高いの方が良いかな？</h4><br />");
} elseif ($guess > $number) {
    print ("<h4>もっと小さいの方が良いかな？</h4><br />");
} else {
    print ("<h4>それは違う！</h4><br />");
}

?>
<form action="<?=$_SERVER['PHP_SELF'] ?>" method="post" name="guess-a-number">
    <label for="guess"></label><br/ >
    <input type="text" name="guess" />
    <input name="number" type="hidden" value="<?= $number ?>" />
    <input name="submit" type="submit" />
</form>
</center>
</body>
</html>
