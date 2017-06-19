# Fake Windows Login

(BETA - In Development)



For Windows instalations using a custom login background please navigate to the following local file path:
- C:\\Windows\System 32\oobe\Info\Backgrounds
Then upload the image named BackgroundDefault.jpeg to your root directory path.
Then rename to bg.png

For Windows instilations connected to a network domain please modify the folowing line:
- /index.xhtml:
	154: <p class="domain"> Domain: ________</p>

If you  are not connected to a domain please remove the following lines:
- /index.xhtml:
    154: <p class="domain"> Domain: _______</p>
    155: <p class="domainlog"> How do I log in to another domain?</p>

For windows instalations where the red shutdown button is displayed, un-comment the following lines:



For windows instalations with profile pictures please do the following:
- navigate to control pannel --> User Accounts and Family Safty --> User Accounts
- Take a screen shot of that user picture and remove all whitespace and add a transparent background.
- Then upload that image t your root directory and name it profile.png


To start from bash:

$ /etc/init.d/apache2 start


Origional Authors:
- Nate Goldsborough     
- Seth Traman