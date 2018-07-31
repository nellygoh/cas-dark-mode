# CAS Dark Mode Theme for Slack Desktop App
Credit to: [Jonathan la Cour](https://github.com/laCour/slack-night-mode)


## Installation
**Windows User**: 
1. Open a new File Explorer Window, and copy/paste the code below on the address bar
```
%LocalAppData%/slack/app-3.2.0/resources/app.asar.unpacked/src/static
```

2. Look for the file name **ssb-interop.js**, right click on the file, and choose 'Open with' -> Notepad

3. Copy/paste the code below on the last line of the code file. **_Please do not remove or edit the core code._**
```
document.addEventListener('DOMContentLoaded', function() {
 $.ajax({
   url: 'https://raw.githubusercontent.com/nellywg/CSS/master/cas-dark-mode.css',
   success: function(css) {
     $("<style></style>").appendTo('head').html(css);
   }
 });
});
```

4. Go back to your Slack app, and press <kbd>Ctrl</kbd> + <kbd>R</kbd> on your keyboard to see the change OR restart your slack.

Enjoy :sunglasses:
