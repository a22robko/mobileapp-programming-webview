
# Rapport

Besrkvining:
Först hade man som uppgift att “Forka”. När man forkar skapar man en kopia av appen i min 
egna github som jag senare kunde ändra och arbeta med. Sen klonade jag appen för att senare 
kunna öppna den i Android Studio så där öppnades den och jag började ändra koden och följa 
uppgiftsbeskrivningen. Det första som jag skulle göra var att ändra textsträngen, då var man 
tvungen att göra det i strings.xml. För att ta sig dit var man tvungen att trycka på values 
mappen.Sen när det var klart sa uppgiftsbeskrivningen att man skulle aktivera internetåtkomsten 
det gjorde man i AndroidManifest.xml. Sen skapades man ett WebView element i layoutfilen 
som heter actvity main.xml. Detta gjorde jag genom att byta ut den befintliga 
Textview komponenten som fanns i appens huvudlayouft och i den fanns en 
standardkomponent som heter Textview, det var denna komponent som byttes ut. 
Detta för att kunna visa upp webbsidorna. Sen då gav man Webviews elementet ett ID genom 
att använda sig av: android:id="@+id/my_webview". Sen säger uppgiften att man skall skapa 
en privat medlemsvariabel med typ webView och sedan instansiera den i onCreate(). Senare 
skapades en WebViewClient och till sist var man tvungen att skapa en javascript körning i 
WebVuewClient samt lades en html sida in. Man var tvungen att implenetera funktionerna 
showExternaWebPage() samt ShowInternalWebPage(). 

Förklara kod:

Här skapas WebView med findViewById(). Detta fungerar genom att använda sig av 
TextView som konverteras till WebView.
        myWebView = (WebView) findViewById(R.id.Robin);


Sen skapas WebView instans och tilldelas till Webview med hjälp av 
WebviewClient().Denna hjälper med navigationen för WebView.
        myWebView.setWebViewClient(new WebViewClient());


Till slut lägger man in Javascript som akteiverar WEbview med hjälp av 
getSettings() som man senare ställer in i javaScriptEnabled till true
        myWebView.getSettings().setJavaScriptEnabled(true);


Internal:
![]("Bild1.png")
External:
![]("Bild2.png")

Fördel:
Det var lätt att följa instruktionerna som fanns i canvas samt att det var simpelt att
hitta runt i android appen.

och nackdel: 
Att datorn laggar väldigt mycket eftersom min mac inte klarar av programmet. 


