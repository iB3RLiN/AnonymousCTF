# Anonymous CTF


<div>
حل روم Anonymous من try hack me

</div>

<div>
مستوى الصعوبة: متوسط
</div>

___________________________________________________

<div>
في البداية راح نسوي فحص للمنافذ

![nmap](https://user-images.githubusercontent.com/73380139/192084218-027904cb-557d-4c36-a67e-b5b6cc05cac0.png)

مافي شي مثير للاهتمام غير ftp
</div>

<div>
نسجل دخول ftp Anonymous

![ftp](https://user-images.githubusercontent.com/73380139/192085989-eb7e0b3d-ddd6-48d1-820a-3dc200b8df1b.png)


نشوف فولدر السكربت
</div>

<div>

![ftpScript](https://user-images.githubusercontent.com/73380139/192086206-1c8b0395-9dd8-4492-ab60-ade2508d501d.png)

حصلت ملف نصي غير مهم وملف سكربت باش يتنفذ بشكل تلقائي 

</div>


<div>

بعد شوي بحث عن revers shell
عشان نسوي اتصال عكسي من خلال net cat 

![pyShell](https://user-images.githubusercontent.com/73380139/192088910-d6b54f3b-5d7f-428f-a3c4-ab0d877dcc23.png)
 
 او شوف shell يناسب من خلال الرابط
 
https://www.hackingtutorials.org/networking/hacking-netcat-part-2-bind-reverse-shells/

</div>

<div>
الحين نرجع نرفع الملف في نفس المكان 

![put](https://user-images.githubusercontent.com/73380139/192088715-19ea4abb-7f86-4e63-95cc-95d4306d6879.png)

</div>

<div>
نفتح اتصال nc وننتطر شوي وراح يتصل فينا الـshell بشكل عكسي 
وراح نحصل علم اليوزر user flag

![userFlag](https://user-images.githubusercontent.com/73380139/192089066-30ec21f7-203d-4464-9a94-4451bc7b8ef1.png)

</div>

<div>
الحين راح نصعد صلاحياتنا لروت 

![privScToRoot](https://user-images.githubusercontent.com/73380139/192089223-a6e2bdfe-dbc9-46d5-8542-e9d64f25b01d.png)


![findPermPath](https://user-images.githubusercontent.com/73380139/192089186-5ebea070-f6d7-4e43-80a1-79c64b497622.png)

اخذنا الصلاحيات 

![imRoot](https://user-images.githubusercontent.com/73380139/192089308-a8553078-fc84-48f7-a1c7-4830568e3dc3.png)

وهذا العلم root flag

![rootFlag](https://user-images.githubusercontent.com/73380139/192089344-98de50a5-7de0-4f96-a885-fdc2d8136fb3.png)


</div>

<div>
المراجع 

https://gtfobins.github.io/gtfobins/env/

https://www.hackingtutorials.org/networking/hacking-netcat-part-2-bind-reverse-shells/
</div>

