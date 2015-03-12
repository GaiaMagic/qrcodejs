# QRCode.js

QRCode.js is a JavaScript QRCode library without any dependency.

Fork of <https://github.com/davidshimjs/qrcodejs>.

* Removed SVG and table drawer.
* Added `margin` option. (normally, if you save the QR code
image on your phone and if the background color of the photo
viewer on the Android phone is also black, then the QR code
can not be scanned; adding a white margin fixes this problem)

Needs IE 9+.

## Basic Usages

```
<div id="qrcode"></div>
<script type="text/javascript">
var qrcode = new QRCode(document.getElementById("qrcode"), {
	text:         "http://jindo.dev.naver.com/collie",
	width:        128,
	height:       128,
	colorDark:    "#000000",
	colorLight:   "#ffffff",
	correctLevel: QRCode.CorrectLevel.H
	margin:       0
});
</script>
```

## License

MIT License
