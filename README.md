# App-redirect-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>App Redirect</title>
    <script>
        function redirectToStore() {
            var userAgent = navigator.userAgent || navigator.vendor || window.opera;
            if (/android/i.test(userAgent)) {
                window.location.href = "(https://play.google.com/store/search?q=youtube&c=apps&hl=ko)";
            } else if (/iPad|iPhone|iPod/.test(userAgent) && !window.MSStream) {
                window.location.href = "(https://apps.apple.com/kr/app/youtube/id544007664)"
            }
        }
        window.onload = redirectToStore;
    </script>
</head>
<body>
    <p>Redirecting...</p>
</body>
</html>
