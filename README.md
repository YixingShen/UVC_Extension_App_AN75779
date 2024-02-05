# UVC_Extension_App_AN75779

# Re: UVC Extension unit

The AN75779 App note firmware implements a UVC extension unit. Refer the App note for more details on the firmware implementation. A sample extension unit control- Get or set device firmware version is implemented in the AN75779 firmware. A host application needs to be designed to communicate with the extension unit of this firmware. The Windows host application is based on the Microsoft’s Media foundation class (MMF) and DirectShow (DSHOW) APIs. More details are available at msdn.microsoft.com and docs.microsoft.com.

The sample host application (Console App) attached with this post is built with Visual studio 2015 (VS 2015). If there are problems compiling the attached project, develop a new application in VS 2015. Follow these steps:

1. Make a new console app project with pre-compiled headers.

2. Use the UVCExtensionApp.c and .h files.

3. In liker > Input > Additional Dependencies, include library files mf.lib, mfreadwrite.lib, mfplat.lib, mfplay.lib and mfuuid.lib. Microsoft SDK must be installed to use mflpay, mfreadwrite, etc. library files.

NOTE: Cypress will not entertain any requests to change/update the host application. User is responsible to design their own application based on their requirements. The attached project is just for reference.