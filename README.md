requirement
Flask==2.0.3
SQLAlchemy==1.4.31

template index
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>URL Shortener</title>
</head>
<body>
    <h1>URL Shortener</h1>
    <form method="post">
        <label for="original_url">Enter URL:</label>
        <input type="text" id="original_url" name="original_url" required>
        <button type="submit">Shorten</button>
    </form>
</body>
</html>
