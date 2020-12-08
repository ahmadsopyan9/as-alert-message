# as-alert-message
 AsAlertMessage is a simple, sweet, customizable, animated modal plugin used to replace the default alert / prompt / confirm dialog boxes. AsAlertMessage is independent of jquery
 
<a href="https://plugin.isfidev.net/asalertmessage/demo.html" target="_blank"> See Demo Here</a>

<img src="https://raw.githubusercontent.com/ahmadsopyan9/as-alert-message/main/screenshot.png">

## Usage
```html
<link href="css/as-alert-message.min.css" rel="stylesheet">
<script src="js/as-alert-message.min.js"></script>
```

## Example Code

#### Create Basic Alert
```html
asAlertMsg("hey test text");
```

#### Alert automatically close
```html
asAlertMsg({
  "title": "Title message",
  "message": "Text message"
});
```

#### Alert with button to close
```html
asAlertMsg({
  "title": "Title message",
  "message": "Text message",
  "button": {
  	"title": "Title Button",
  	"bg": "success"
  }
});
//for button
//default {}
//title & bg, is optional
```

#### Alert with button to redirect
```html
asAlertMsg({
  "type": "success",
  "title": "Title message",
  "message": "Text message",
  "button": {
  	"title": "Title Button",
  	"bg": "success"
  },
  "success": {
	"redirect": ["https://google.com"]
  }
});
```

#### Alert with automatically redirect
```html
asAlertMsg({
  "type": "success",
  "title": "Title message",
  "message": "Text message",
  "timer": 1000,
  "success": {
	"redirect": ["https://google.com"]
  }
});
//for this timer parameter the optional
//default is 1500
```

#### If you want to redirect to a new tab, add "_blank" to the redirect parameter value, like this 
```html
"redirect": ["https://google.com","_blank"]
```
