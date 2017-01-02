## Write the Difference in between high-level UI with Low-Level UI.
High-level UI APIs | Low-level UI APIs| 
------------ | ------------- | 
Support widget-based model. A widget is a re-usable UI component, such as buttons and text boxes. | Support pixel-based model.  
Contain several classes, such as Screen and Item. These classes help create UIs components, such as buttons, for mobile devices. | Contain four classes: Canvas, Graphics, Font, and Image. These classes help to control the screen by using UI components, such as canvas.  
Provide the portability feature, which enables you to use the same high-level UI API to create UIs for several mobile devices. | Provide device specific support for creating UIs. As a result, you cannot use the same low-level API to create UIs for different mobile devices. 
Restrict you from controlling the display screen of a mobile device.| Provide methods to control the display screen of a mobile device. For example, you can change the font of a text by using the methods of the low-level APIs. 
Do not control the user inputs to a mobile device.| Enable you to control the user inputs to a mobile device.Provide support for structured screens. | Provide support for unstructured screens.

## Explain the Components of CLDC
* CLDC library
* Kilobyte Virtual Machine (KVM)
* Java programming language 

### CLDC Library
The CLDC library contains a minimum useful set of APIs that support application development and profile definition. CLDC also contains some extra libraries to support networking capabilities in mobile devices. 
### Kilobyte Virtual Machine(KVM)KVM represents the virtual machine for small devices that implemented CLDC. The KVM is also compliant with JVM, which is used in J2SE edition but has limited features as compared to JVM. (Difference between kvm jvm)
## Explain various kinds of Wireless Technologies.* General Packet Radio Service (GPRS)* Third Generation GSM (3GSM)* Enhanced Data rates for GSM Evolution (EDGE)* Wireless Application Protocol (WAP)### GPRSGPRS is a data service used to send and receive data across the wireless network. GPRS enables mobile devices to connect instantly to the server so that the application can access the required data. GPRS allows you to download wireless applications on mobile devices. It also provides the facility to deliver textual and visual information, such as sports scores, news headlines, and weather information. In addition, you can also send and receive still and animated images by using GPRS. ### 3GSM3GSM is an enhanced version of the GSM platform that provides third generation mobile multimedia services. 3GSM provides high bandwidth and quality for transmitting voice and text across a wireless network. 3GSM uses an additional radio signal, which was not available in the GSM platform. This additional radio signal provides added bandwidth, which enables mobile device subscribers to access high data transmission speed and multimedia data services.3GSM technology provides advanced multimedia services and greater bandwidth that is not provided by GPRS wireless technology.### EDGEEDGE is a 3rd Generation (3G) wireless technology that provides broader bandwidth and faster data transfer in mobile devices. This technology enables mobile users to download video and music clips and access high-speed Internet. End users, by using the EDGE wireless technology, can connect to the Internet and exchange data faster than by using the 2nd Generation (2G) wireless technology. The first generation of wireless technology, known as 1G, used analog voice signaling to transfer voice-based data in mobile devices. The second generation of wireless technology, known as 2G, used digital voice encoding to transfer voice-based data. The third generation of wireless technology, known as 3G, provides advanced features, such as enhanced multimedia, broad bandwidth, and high-speed data access### WAPWireless Application Protocol (WAP) is a specification that adapts several data‑handling techniques used by Web protocols such as TCP/IP. The development of WAP applications is relatively simple because it reuses existing Web technologies. To generate dynamic WAP content, you can use either Servlets and Java Server Pages (JSP) or Wireless Markup Language (WML). Although WAP and J2ME are complementary technologies, they operate in different ways. When using the WAP technology, the mobile device runs a browser that accesses the intranet or Internet applications. The mobile device does not contain any other application. In a J2ME enabled mobile device, you need to download an application and run it locally on the device. You do not need to use a browser to access an application. ##  Explain JAD File and its components.
JAD: Java Application Descriptor   
*	MIDlet-Name*	MIDlet-Version*	MIDlet-Vendor*	MIDlet-<n> for each MIDlet*	MIDlet-Jar-URL*	MIDlet-Jar-Size## Explain the usage of Obfuscating the MIDlet.Obfuscation refers to the process of reducing the size of the Java byte code of a MIDlet application. Obfuscation helps in reducing the time required to download the MIDlet application in a mobile device. It also helps in securing the Java source code of a MIDlet application.     
The compiled class files of Java can be reverse engineered to produce the Java source files by using a tool called a decompiler. This is a threat to the Java source files. Obfuscation prevents this threat by preventing reverse engineering.     
The Obfuscation process removes information such as comments, line numbers, and local variable names present in the Java source files. After this information is removed, any attempt at reverse engineering is not successful. This is because the information that is derived after decompiling the Java source files becomes very difficult to understand. ## List the differences between KVM and JVM
Java Language Features | KVM | JVM
-----------------------|-----|----
Java Native Interface (JNI) | Does not support JNI. | Supports JNI Includes features to reduce the cost of implementation of virtual machine.
Thread groups|Does not support thread groups. Thread operations, such as starting and stopping a thread, can only be applied to individual thread objects. |Supports thread groups.
Reflection features | Does not support reflection features. Reflection features help you to inspect the number and content of classes, such as objects, methods, fields, threads, and other runtime structures in the virtual machine. | Supports reflection features.
Class file verification | Performs class verification in two steps, preverification and in-device verification. Preverification is performed before downloading a class file into a mobile device. In‑device verification occurs after preverification is completed. | Performs class verification only once, during compilation of Java classes.
## List the requirements of CLDC specification.*	160 KB of non-volatile memory for the virtual machine and CLDC libraries(ROM)*	32 KB of volatile memory for the virtual machine(RAM)*	16-bit or 32-bit processor *	Wireless network connection of limited bandwidth, such as Bluetooth and GPRS## Explain all the classes derived from the Screen Class. 
* Textbox 
* List
* Alert
* Form -> Item -> ...

## Explain states of the Life Cycle of MIDlet*	Active state: Indicates the state when a MIDlet initially starts after it is launched by the AMS. This state is defined by the startApp() method of the MIDlet class.*	Paused state: Indicates the state when a MIDlet is stopped temporarily. This state is defined by the pauseApp() method of the MIDlet class.*	Destroyed state: Indicates the state when a MIDlet is permanently destroyed from the mobile device. When a MIDlet is destroyed, it cannot be reused. This state is defined by the destroyApp() method of the MIDlet class.##  Explain all the three attributes of Command class.Method | Description
-------| ----------GetCommandType()|Returns an int value to indicate the type attribute of the current Command object.getLabel()|Returns the label of the Command object.getLongLabel()|Returns the long label of the Command object. Long label provides additional information, such as the function of the Command object.getPriority()|Returns an int value to specify the priority of the Command object. 