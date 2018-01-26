Work Log
*************************
Project: Autho_MSV
*************************

Run the app and register/login with 2FA and visual code

Add: > bower install qrcode-js ("qrcode-js" : "*")   Don't use: NuGet OR npm not yet!

Follow online instructions : https://docs.microsoft.com/en-us/aspnet/core/security/authentication/identity-enable-qrcodes

In Pages\Account\Manage\EnableAuthenticator.cshtml (Razor Pages) or Views\Manage\EnableAuthenticator.cshtml (MVC), locate the Scripts section at the end of the file:

TIP for <script type="text/javascript" src="~/lib/qrcode-js/qrcode.js"></script> use auto complete

Run again and see the bar code

Remove the blue box instructions!

TIP In dev authenicator: https://gauth.apps.gbraad.nl/

See image: test.png

**************************************
* Now use external Authentication
**************************************
REF DOCS: https://docs.microsoft.com/en-us/aspnet/core/security/authentication/social/index

NOTE: DO NOT USE appjsonsettings.json for secrets DO USE secrets.json

Solution > context menu > Manage User Secrets

"Authentication:Microsoft:ApplicationId": "...",
"Authentication:Microsofy:Password":  "..."

**************************************
* Introduction to Authorization
**************************************