# Alerta Donaciones

Para que comiencen a aparecer las alertas en tu pagina web solo pon el código dentro del tag `<body>`

```
<style>
body{margin-top:100px}.donation-alert{color:#FFF;padding:20px 80px;transform:translateY(-100%);transition:all ease 1s;position:fixed;top:0;left:0;z-index:9999;width:100%;height:80px}.donation-alert a{background:rgba(0,0,0,.1);border:2px solid #FFF;color:#fff!important;-webkit-border-radius:7px;border-radius:7px;padding:10px 20px;transition:all .2s linear;float:right;display:none;font-size:1rem}.donation-alert h2{display:none;font-size:1.5em}.donation-alert a:hover{background:rgba(0,0,0,.5);cursor:pointer}.donation-alert.in{max-height:500px;transform:translateY(0);background-color:#F73535!important}.donation-alert.in a,.donation-alert.in h2{display:inline}@media screen and (max-width:768px){.donation-alert{padding:20px}}@media screen and (max-width:425px){body{ margin-top: 200px; }.donation-alert{height:auto}.donation-alert h2{display:block}.donation-alert a{float:none;display:block!important;text-align:center;margin-top:30px}}
</style>

<div class="donation-alert" role="alert" id="alert" >
<h2>Ayudemos a los afectados por el sismo.</h2>
<a href="https://www.paypal.com/mx/webapps/mpp/donar/institution?name=redCross" target="_blank">Haz tu donativo en segundos</a>
</div>

<script>
var alertEl = document.getElementById("alert");

setTimeout(function(){ 
alertEl.className += " in"; 
}, 1000);
</script>
```

