---?image=assets/images/gitpitch-audience.jpg
@title[Platform Build Win Lab]
<br><br><br><br>
## <span class="gold"   >UEFI & EDK II Training</span>

#### UEFI HII Overview
UEFI Human Interface Infrastructure (HII)

<br>
<span style="font-size:0.75em" ><a href='http://www.tianocore.org'>tianocore.org</a></span>
Note:
  PITCHME.md for UEFI / EDK II Training   UEFI HII Overview Pres

  Copyright (c) 2018, Intel Corporation. All rights reserved.<BR>

  Redistribution and use in source (original document form) and 'compiled'
  forms (converted to PDF, epub, HTML and other formats) with or without
  modification, are permitted provided that the following conditions are met:

  1) Redistributions of source code (original document form) must retain the
     above copyright notice, this list of conditions and the following
     disclaimer as the first lines of this file unmodified.

  2) Redistributions in compiled form (transformed to other DTDs, converted to
     PDF, epub, HTML and other formats) must reproduce the above copyright
     notice, this list of conditions and the following disclaimer in the
     documentation and/or other materials provided with the distribution.

  THIS DOCUMENTATION IS PROVIDED BY TIANOCORE PROJECT "AS IS" AND ANY EXPRESS OR
  IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
  MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO
  EVENT SHALL TIANOCORE PROJECT  BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
  SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
  PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
  WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
  OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS DOCUMENTATION, EVEN IF
  ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.



---  
@title[Lesson Objective]
<BR>
### <p align="center"<span class="gold"   >Lesson Objective </span></p><br>
<!---  Add bullets using https://fontawesome.com/cheatsheet certificate
-->
 @fa[certificate gp-bullet-green]<span style="font-size:0.9em">&nbsp;&nbsp;What is the Infrastructure for HII </span><br><br>
 @fa[certificate gp-bullet-cyan]<span style="font-size:0.9em">&nbsp;&nbsp;How Does HII Work </span><br><br>
 @fa[certificate gp-bullet-yellow]<span style="font-size:0.9em">&nbsp;&nbsp;Lab for HII</span> <br><br>
  


---?image=assets/images/binary-strings-black2.jpg
@title[User Interface HII Overview Section]
<br><br><br><br><br>
## <span class="gold"  >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;UI HII Overview </span>
<span style="font-size:0.9em" > &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;User Interface HII Overview</span>


---?image=/assets/images/slides/Slide4.JPG
@title[Why HII]
### <p align="right"><span class="gold" >Why?</span></p>

Note:
- Single window for full platform configuration 
- Avoid multiple hotkeys
- Localization support
- Unified look and feel
- If driver supports any configuration, must be implemented using HII
- Expose content to be seamlessly integrated in platform solutions



---?image=/assets/images/slides/Slide5.JPG
<!-- .slide: data-transition="none" -->
@title[HII: Key Concepts]
### <p align="center"><span class="gold" >HII: Key Concepts</span></p>

Note:
- Solve problems from legacy BIOS …
  - Different menus for BIOS setup & OpROM
  - User has problems finding the right menu
  - OEMs need a consistent user interface
- UEFI Human Interface Infrastructure (HII)
  - System firmware has a common setup browser
  - Drivers don’t carry their own UI
  - Single point for pre-OS setup interface
  - Firmware & Drivers publish to a “database”

+++?image=/assets/images/slides/Slide6.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->

@title[HII: Key Concepts 02]
### <p align="center"><span class="gold" >HII: Key Concepts</span></p>

Note:
- Solve problems from legacy BIOS …
  - Different menus for BIOS setup & OpROM
  - User has problems finding the right menu
  - OEMs need a consistent user interface
- UEFI Human Interface Infrastructure (HII)
  - System firmware has a common setup browser
  - Drivers don’t carry their own UI
  - Single point for pre-OS setup interface
  - Firmware & Drivers publish to a “database”


+++?image=/assets/images/slides/Slide7.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->

@title[HII: Key Concepts 03]
### <p align="center"><span class="gold" >HII: Key Concepts</span></p>

Note:
- Solve problems from legacy BIOS …
  - Different menus for BIOS setup & OpROM
  - User has problems finding the right menu
  - OEMs need a consistent user interface
- UEFI Human Interface Infrastructure (HII)
  - System firmware has a common setup browser
  - Drivers don’t carry their own UI
  - Single point for pre-OS setup interface
  - Firmware & Drivers publish to a “database”


+++?image=/assets/images/slides/Slide8.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->

@title[HII: Key Concepts 04]
### <p align="center"><span class="gold" >HII: Key Concepts</span></p>

Note:
- Solve problems from legacy BIOS …
  - Different menus for BIOS setup & OpROM
  - User has problems finding the right menu
  - OEMs need a consistent user interface
- UEFI Human Interface Infrastructure (HII)
  - System firmware has a common setup browser
  - Drivers don’t carry their own UI
  - Single point for pre-OS setup interface
  - Firmware & Drivers publish to a “database”


+++?image=/assets/images/slides/Slide9.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->

@title[HII: Key Concepts 05]
### <p align="center"><span class="gold" >HII: Key Concepts</span></p>

Note:
- Solve problems from legacy BIOS …
  - Different menus for BIOS setup & OpROM
  - User has problems finding the right menu
  - OEMs need a consistent user interface
- UEFI Human Interface Infrastructure (HII)
  - System firmware has a common setup browser
  - Drivers don’t carry their own UI
  - Single point for pre-OS setup interface
  - Firmware & Drivers publish to a “database”


+++?image=/assets/images/slides/Slide10.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->

@title[HII: Key Concepts 02]
### <p align="center"><span class="gold" >HII: Key Concepts</span></p>

Note:
- Solve problems from legacy BIOS …
  - Different menus for BIOS setup & OpROM
  - User has problems finding the right menu
  - OEMs need a consistent user interface
- UEFI Human Interface Infrastructure (HII)
  - System firmware has a common setup browser
  - Drivers don’t carry their own UI
  - Single point for pre-OS setup interface
  - Firmware & Drivers publish to a “database”


---?image=/assets/images/slides/Slide11.JPG
@title[Design Discussions]
### <p align="right"><span class="gold" >Design Discussions</span></p>
 
Note:
- The example on the right shows a basic platform configuration or “setup” model. 
- The drivers and applications install elements (such as fonts, strings, images and forms) into the HII Database, which acts as a central repository for the entire platform. The Forms Browser uses these elements to render the user interface on the display devices and receive information from the user via HID devices. When complete, the changes made by the user in the Forms Browser are saved, either to the EFI global variable storage—(GetVariable() and  SetVariable()— or to variable storage provided by the individual drivers

- TOP
  - Platform and Standard User Interactions

- Bottom
  - There are various scenarios where a platform component must interact in some fashion with the user. Examples of this are when presenting a user with several choices of information (e.g. boot menu) and sending information to the display (e.g. system status, logo, etc).



---?image=assets/images/binary-strings-black2.jpg
@title[HII Components Section]
<br><br><br><br><br>
## <span class="gold"  >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HII Components </span>
<span style="font-size:0.9em" > &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;User Interface HII Overview</span>
 


---?image=/assets/images/slides/Slide13.JPG
<!-- .slide: data-transition="none" -->
@title[HII Components]
### <p align="right"><span class="gold" >HII Components</span></p>

Note:
- Strings are represented by string tokens.  They are listed in a table and referenced by a token number.  This results in multiple language support.  Depending the language, different tables are accessed.
- Fonts
  - Presumption of bitmap fonts for easier localization (GraphicsConsoleDxe).
- Keyboard
  - Keyboard Mapping (UsbKb)
- Forms
  - Describe user interface layout for ‘windowing’ interfaces
  - An application that uses String and Font support
- Package
  - Self supporting data structure containing fonts, strings, and forms from a driver or set of drivers

+++?image=/assets/images/slides/Slide14.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->
@title[HII Components 02]
### <p align="right"><span class="gold" >HII Components</span></p>

Note:
- Strings are represented by string tokens.  They are listed in a table and referenced by a token number.  This results in multiple language support.  Depending the language, different tables are accessed.
- Fonts
  - Presumption of bitmap fonts for easier localization (GraphicsConsoleDxe).
- Keyboard
  - Keyboard Mapping (UsbKb)
- Forms
  - Describe user interface layout for ‘windowing’ interfaces
  - An application that uses String and Font support
- Package
  - Self supporting data structure containing fonts, strings, and forms from a driver or set of drivers

+++?image=/assets/images/slides/Slide15.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->
@title[HII Components 03]
### <p align="right"><span class="gold" >HII Components</span></p>

Note:
- Strings are represented by string tokens.  They are listed in a table and referenced by a token number.  This results in multiple language support.  Depending the language, different tables are accessed.
- Fonts
  - Presumption of bitmap fonts for easier localization (GraphicsConsoleDxe).
- Keyboard
  - Keyboard Mapping (UsbKb)
- Forms
  - Describe user interface layout for ‘windowing’ interfaces
  - An application that uses String and Font support
- Package
  - Self supporting data structure containing fonts, strings, and forms from a driver or set of drivers

+++?image=/assets/images/slides/Slide16.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->
@title[HII Components 04]
### <p align="right"><span class="gold" >HII Components</span></p>

Note:
- Strings are represented by string tokens.  They are listed in a table and referenced by a token number.  This results in multiple language support.  Depending the language, different tables are accessed.
- Fonts
  - Presumption of bitmap fonts for easier localization (GraphicsConsoleDxe).
- Keyboard
  - Keyboard Mapping (UsbKb)
- Forms
  - Describe user interface layout for ‘windowing’ interfaces
  - An application that uses String and Font support
- Package
  - Self supporting data structure containing fonts, strings, and forms from a driver or set of drivers

+++?image=/assets/images/slides/Slide17.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->
@title[HII Components 05]
### <p align="right"><span class="gold" >HII Components</span></p>

Note:
- Strings are represented by string tokens.  They are listed in a table and referenced by a token number.  This results in multiple language support.  Depending the language, different tables are accessed.
- Fonts
  - Presumption of bitmap fonts for easier localization (GraphicsConsoleDxe).
- Keyboard
  - Keyboard Mapping (UsbKb)
- Forms
  - Describe user interface layout for ‘windowing’ interfaces
  - An application that uses String and Font support
- Package
  - Self supporting data structure containing fonts, strings, and forms from a driver or set of drivers


---?image=/assets/images/slides/Slide18.JPG
@title[HII Strings]
### <p align="right">Strings</p>

Note:
- Strings stored in Unicode
  - Real string encodings required for e.g. VT100
  - Already the text standard in EFI today
- Localization happens at the string level
  - Caller externs and passes in language independent string token
  - String support determines actual string from token and selected language
  - Usage Model:
    - A string library supporting translations
    - Reduces translation costs and delays
    - Tools to extract strings depending on use by driver
    - Analysis of strings used to extract fonts

---?image=/assets/images/slides/Slide19.JPG
@title[Token to String Mapping]
### <p align="right"><span class="gold" >Token to String Mapping</span></p>

Note:
- Request: Print string with token 37
- Currently selected language is as in UEFI 2.X.  This is used to select between language data structures.  (The structures indicate which language(s) they support).
- The top part of the structure maps from token to string. The bottom part of the structure is the strings



---?image=/assets/images/slides/Slide20.JPG
@title[String Example (.uni file)]
### <p align="right"><span class="gold" >String Example (.uni file)</span></p>

Note:
<pre>
 #langdef   en-US  	"English"
 #langdef   fr-FR  	"Francais“
 #langdef   sv-SE	“Svenska”

 #string STR_FORM_SET_TITLE 
        #language en-US "Browser Testcase Engine"
        #language fr-FR "Navigateur Testcase Moteur”
        #language sv-SE "Webbläsare Testcase Motor”
 #string STR_FORM_SET_TITLE_HELP  
        #language en-US "This is a sample UEFI driver which is used to test the browser op-code operations. "
        #language fr-FR “Il s'agit d'une UEFI Driver échantillon qui est utilisé pour tester les navigateurs op-code opérations.“
        #language sv-SE ”Detta är ett exempel på UEFI-drivrutin som används för att testa webbläsaren op-kod operationer”

 #string STR_FORM1_TITLE
        #language en-US "My First Setup Page"
        #language fr-FR "Mi Primero Arreglo Página“ 
        #language sv-SE "Min första inställningssidan”
</pre> 



---?image=/assets/images/slides/Slide21.JPG
@title[HII Fonts]
### <p align="right">Fonts</p>

Note:
- One Standard Font for UEFI
  - One font database accumulated during boot
- Each Component Provides Its Fonts
  - System provides ASCII and ISO Latin-1
  - Fonts only required for characters in strings that may appear
    - If the firmware will never print “tractor” in Kanji, discard the bit image
  - Result is a sparse array of characters indexed by the Unicode ‘weight’
- Wide and Narrow glyphs supported 




---?image=/assets/images/slides/Slide22.JPG
@title[HII Keyboards]
### <p align="right">Keyboards</p>

Note:

- Support varying keyboards
  - UK and US keyboard layout are not the same.  Certainly that is the case for US and Arabic, etc.
  - Adding support of other modifiers (e.g. Alt-GR, Dead-keys, etc)
- Keyboard Layout
  - Allow for a standardized mechanism to describe a keyboard layout and add to system database.
  - Allow for switching keyboard layouts.  



---?image=/assets/images/slides/Slide23.JPG
@title[HII Forms]
### <p align="right">Forms</p>

Note:
- How a UEFI driver or application may present a forms (or dialogs) based interface. The forms-based interface assumes that each window or screen consists of some window dressing (title & buttons) and a list of questions. These questions represent individual configuration settings for the application or driver, although several GUI controls may be used for one question 

- The forms are stored in the HII database, along with the strings, fonts & images
- Other applications may use the information within the forms to validate configuration setting values
- The Forms Browser provides a forms-based user interface which understands 
  - how to read the contents of the forms
  - interact with the user
  - save the resulting values
- The Forms Browser uses forms data installed by an application or driver during initialization in the HII database. 


---?image=/assets/images/slides/Slide24.JPG
@title[Visual Forms Representation (VFR)]
### <p align="right"><span class="gold" >Visual Forms Representation (VFR)</span></p>

Note:
- VFR (Visual Forms Representation) is the development language used to create IFR (Internal Forms Representation). IFR is the compiled version of the control language. This language controls what the contents of each displayed page consists of, where the changed data gets saved, how pages are linked, and much more. 
- VFR source files will include a Unicode file(s) which contains the string definitions for the particular application. The Unicode file will contain both the displayed strings as well as the translations for all the supported languages for the particular application. 

- Language used to describe what a page layout would be in a browser as well as the op-codes and string tokens to display 
- Op-codes are defined for the following functions examples
  - formSet and form definitions
  - One of type questions with corresponding options (combo) fields
```
    checkbox 
    numeric 
    oneof 
    String
```	
  - Boolean expressions in support of errors, suppress, and gray outs
```
  "disableif" 
  “suppressif“
  “grayoutif"  
```


---?image=/assets/images/slides/Slide25.JPG
@title[Form Example (.vfr file)]
### <p align="right"><span class="gold" >Form Example (.vfr file)</span></p>

Note:

<pre>
formset
  guid     = FORMSET_GUID,
  title    = STRING_TOKEN(STR_FORM_SET_TITLE),
  help     = STRING_TOKEN(STR_FORM_SET_TITLE_HELP),
  classguid = EFI_HII_PLATFORM_SETUP_FORMSET_GUID,

 varstore   DRIVER_SAMPLE_CONFIGURATION, 
	name = MyIfrNVData,
	guid = FORMSET_GUID;

 form formid = 1,
       title  = STRING_TOKEN(STR_FORM1_TITLE);  

 oneof varid  = MyIfrNVData.MyVariableForOneofPrompt,
  prompt      = STRING_TOKEN(STR_ONE_OF_PROMPT),
   help       = STRING_TOKEN(STR_ONE_OF_HELP),
  option text = STRING_TOKEN(STR_ONE_OF_TEXT1), value = 0x0, flags = 0;
  option text = STRING_TOKEN(STR_ONE_OF_TEXT2), value = 0x1, flags = 0;
  option text = STRING_TOKEN(STR_ONE_OF_TEXT3), value = 0x2, flags = DEFAULT;
 endoneof;
                         • • •
 endform;
endformset;
</pre>


---?image=/assets/images/slides/Slide26.JPG
@title[Internal Forms Representation (IFR)]
### <p align="right"><span class="gold" >Internal Forms Representation (IFR)</span></p>

Note:
- Internal Forms Representation created by VFR to IFR tool
- Byte encoded operations (much smaller)
- String references abstracted as tokens
- Improved validation, visibility primitives
- At better level of presentation control for firmware
  - Tension between configuration driver and presentation driver over control of presentation format
- Easy to
  - Interpret for small Setup engine in desktop firmware
  - Translate into XHTML or JavaScript or … 



---?image=/assets/images/slides/Slide27.JPG
<!-- .slide: data-transition="none" -->
@title[Minimum Files for HII Driver]
### <p align="right"><span class="gold" >Minimum Files for HII Driver</span></p>

Note:
- Driver source file  
  - Consumes HII protocols
  - Produces EFI_HII_CONFIGURATION_ACCESS_PROTOCOL
- Driver include file 
  - Defines data structures
- Strings file 
  - Defines strings in different languages
- Forms file  
  - Defines the layout of the screen 
- Pre-Make file 



+++?image=/assets/images/slides/Slide28.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->
@title[Minimum Files for HII Driver 02]
### <p align="right"><span class="gold" >Minimum Files for HII Driver</span></p>

Note:
- Driver source file  
  - Consumes HII protocols
  - Produces EFI_HII_CONFIGURATION_ACCESS_PROTOCOL
- Driver include file 
  - Defines data structures
- Strings file 
  - Defines strings in different languages
- Forms file  
  - Defines the layout of the screen 
- Pre-Make file 


+++?image=/assets/images/slides/Slide29.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->
@title[Minimum Files for HII Driver 03]
### <p align="right"><span class="gold" >Minimum Files for HII Driver</span></p>

Note:
- Driver source file  
  - Consumes HII protocols
  - Produces EFI_HII_CONFIGURATION_ACCESS_PROTOCOL
- Driver include file 
  - Defines data structures
- Strings file 
  - Defines strings in different languages
- Forms file  
  - Defines the layout of the screen 
- Pre-Make file 


+++?image=/assets/images/slides/Slide30.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->
@title[Minimum Files for HII Driver 03]
### <p align="right"><span class="gold" >Minimum Files for HII Driver</span></p>

Note:
- Driver source file  
  - Consumes HII protocols
  - Produces EFI_HII_CONFIGURATION_ACCESS_PROTOCOL
- Driver include file 
  - Defines data structures
- Strings file 
  - Defines strings in different languages
- Forms file  
  - Defines the layout of the screen 
- Pre-Make file 


---?image=/assets/images/slides/Slide31.JPG
<!-- .slide: data-transition="none" -->
@title[EDK II HII]
### <p align="right"><span class="gold" >EDK II HII</span></p>

Note:
- The EFI Configuration Driver is the program that reads the contents of the HII Database and interprets the data to present it to the user. This is also the program that takes the user input and provides for a mechanism to save the changes into an NVRAM location. 
- There is an assumption of having some type of NVRAM available so that settings that are changed by the user are able to be saved. How one gets to the NVRAM is based on whether it is system NV storage one is accessing, or NV storage local to a specific card. Both are supported. 
- With the exception of setting a system password, and system date and time, settings are not posted to NV storage until the user directs the infrastructure specifically to do so. As a rule of thumb, hardware configuration changes do not take place until a system reset has occurred. 

- HiiConfigAccess Protocol. Read/Write/CallBack().


+++?image=/assets/images/slides/Slide32.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->
@title[EDK II HII 02]
### <p align="right"><span class="gold" >EDK II HII</span></p>

Note:
- The EFI Configuration Driver is the program that reads the contents of the HII Database and interprets the data to present it to the user. This is also the program that takes the user input and provides for a mechanism to save the changes into an NVRAM location. 
- There is an assumption of having some type of NVRAM available so that settings that are changed by the user are able to be saved. How one gets to the NVRAM is based on whether it is system NV storage one is accessing, or NV storage local to a specific card. Both are supported. 
- With the exception of setting a system password, and system date and time, settings are not posted to NV storage until the user directs the infrastructure specifically to do so. As a rule of thumb, hardware configuration changes do not take place until a system reset has occurred. 

- HiiConfigAccess Protocol. Read/Write/CallBack().


+++?image=/assets/images/slides/Slide33.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->
@title[EDK II HII 03]
### <p align="right"><span class="gold" >EDK II HII</span></p>

Note:
- The EFI Configuration Driver is the program that reads the contents of the HII Database and interprets the data to present it to the user. This is also the program that takes the user input and provides for a mechanism to save the changes into an NVRAM location. 
- There is an assumption of having some type of NVRAM available so that settings that are changed by the user are able to be saved. How one gets to the NVRAM is based on whether it is system NV storage one is accessing, or NV storage local to a specific card. Both are supported. 
- With the exception of setting a system password, and system date and time, settings are not posted to NV storage until the user directs the infrastructure specifically to do so. As a rule of thumb, hardware configuration changes do not take place until a system reset has occurred. 

- HiiConfigAccess Protocol. Read/Write/CallBack().


+++?image=/assets/images/slides/Slide34.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->
@title[EDK II HII 04]
### <p align="right"><span class="gold" >EDK II HII</span></p>

Note:
- The EFI Configuration Driver is the program that reads the contents of the HII Database and interprets the data to present it to the user. This is also the program that takes the user input and provides for a mechanism to save the changes into an NVRAM location. 
- There is an assumption of having some type of NVRAM available so that settings that are changed by the user are able to be saved. How one gets to the NVRAM is based on whether it is system NV storage one is accessing, or NV storage local to a specific card. Both are supported. 
- With the exception of setting a system password, and system date and time, settings are not posted to NV storage until the user directs the infrastructure specifically to do so. As a rule of thumb, hardware configuration changes do not take place until a system reset has occurred. 

- HiiConfigAccess Protocol. Read/Write/CallBack().


+++?image=/assets/images/slides/Slide35.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->
@title[EDK II HII 05]
### <p align="right"><span class="gold" >EDK II HII</span></p>

Note:
- The EFI Configuration Driver is the program that reads the contents of the HII Database and interprets the data to present it to the user. This is also the program that takes the user input and provides for a mechanism to save the changes into an NVRAM location. 
- There is an assumption of having some type of NVRAM available so that settings that are changed by the user are able to be saved. How one gets to the NVRAM is based on whether it is system NV storage one is accessing, or NV storage local to a specific card. Both are supported. 
- With the exception of setting a system password, and system date and time, settings are not posted to NV storage until the user directs the infrastructure specifically to do so. As a rule of thumb, hardware configuration changes do not take place until a system reset has occurred. 

- HiiConfigAccess Protocol. Read/Write/CallBack().


+++?image=/assets/images/slides/Slide36.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->
@title[EDK II HII 06]
### <p align="right"><span class="gold" >EDK II HII</span></p>

Note:
- The EFI Configuration Driver is the program that reads the contents of the HII Database and interprets the data to present it to the user. This is also the program that takes the user input and provides for a mechanism to save the changes into an NVRAM location. 
- There is an assumption of having some type of NVRAM available so that settings that are changed by the user are able to be saved. How one gets to the NVRAM is based on whether it is system NV storage one is accessing, or NV storage local to a specific card. Both are supported. 
- With the exception of setting a system password, and system date and time, settings are not posted to NV storage until the user directs the infrastructure specifically to do so. As a rule of thumb, hardware configuration changes do not take place until a system reset has occurred. 

- HiiConfigAccess Protocol. Read/Write/CallBack().



---?image=assets/images/binary-strings-black2.jpg
@title[How: UEFI HII Protocols Section]
<br><br><br><br><br>
## <span class="gold"  >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;How: UEFI HII Protocols </span>
<span style="font-size:0.9em" > &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Sections 29-31  the UEFI 2.x Specification</span>



---?image=/assets/images/slides/Slide38.JPG
<!-- .slide: data-transition="none" -->
@title[HII Database Overview]
### <p align="right"><span class="gold" >HII Database Overview</span></p>

Note:


+++?image=/assets/images/slides/Slide39.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->
@title[HII Database Overview 02]
### <p align="right"><span class="gold" >HII Database Overview</span></p>

Note:


+++?image=/assets/images/slides/Slide40.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->
@title[HII Database Overview 03]
### <p align="right"><span class="gold" >HII Database Overview</span></p>

Note:


+++?image=/assets/images/slides/Slide41.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->
@title[HII Database Overview 04]
### <p align="right"><span class="gold" >HII Database Overview</span></p>

Note:


+++?image=/assets/images/slides/Slide42.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->
@title[HII Database Overview 05]
### <p align="right"><span class="gold" >HII Database Overview</span></p>

Note:


---?image=/assets/images/slides/Slide43.JPG
@title[UEFI HII Protocols]
### <p align="right"><span class="gold" >UEFI HII Protocols</span></p>

Note:
- Font Protocol
	- String to Image, Sting ID to Image, Get Glyph, Get Font Info
- String Protocol
	- New – Get – Set – String
	- Get Language & 2nd Language
- Image Protocol
	- New – Get – Set Image
	- Draw Image, Draw Image ID
- Database Protocol
	- New – Remove- Update – List – Export Lists – Get Handle Package 
	- Register, Unregister Package Notify 
	- Find- Get- Set Keyboard layout


---?image=/assets/images/slides/Slide44.JPG
<!-- .slide: data-transition="none" -->
@title[UEFI Driver Initialization Process ]
### <p align="right"><span class="gold" >UEFI Driver Initialization Process </span></p>

Note:

DXE Phase UEFI 2.1+ Driver  Initialization Process

+++?image=/assets/images/slides/Slide45.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->
@title[UEFI Driver Initialization Process 02]
### <p align="right"><span class="gold" >UEFI Driver Initialization Process </span></p>

Note:

DXE Phase UEFI 2.1+ Driver  Initialization Process


+++?image=/assets/images/slides/Slide46.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->
@title[UEFI Driver Initialization Process 03]
### <p align="right"><span class="gold" >UEFI Driver Initialization Process </span></p>

Note:

DXE Phase UEFI 2.1+ Driver  Initialization Process

+++?image=/assets/images/slides/Slide47.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->
@title[UEFI Driver Initialization Process 04]
### <p align="right"><span class="gold" >UEFI Driver Initialization Process </span></p>

Note:

DXE Phase UEFI 2.1+ Driver  Initialization Process

+++?image=/assets/images/slides/Slide48.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->
@title[UEFI Driver Initialization Process 05]
### <p align="right"><span class="gold" >UEFI Driver Initialization Process </span></p>

Note:

DXE Phase UEFI 2.1+ Driver  Initialization Process

+++?image=/assets/images/slides/Slide49.JPG
<!-- .slide: data-background-transition="none" -->
<!-- .slide: data-transition="none" -->
@title[UEFI Driver Initialization Process 06]
### <p align="right"><span class="gold" >UEFI Driver Initialization Process </span></p>

Note:

DXE Phase UEFI 2.1+ Driver  Initialization Process



---?image=/assets/images/slides/Slide50.JPG
@title[Form Browser Protocols]
### <p align="right"><span class="gold" >Form Browser Protocols </span></p>

Note:

- slide shows how the UEFI Driver interfaces the UEFI protocols to publish its forms, strings, etc...


---?image=assets/images/binary-strings-black2.jpg
@title[Lab Section]
<br><br><br><br><br>
## <span class="gold"  >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Lab for HII </span>
<span style="font-size:0.9em" > &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>

---?image=/assets/images/slides/Slide51.JPG
@title[Lab for HII ]
<br>
<br>
<p align="Left"><span class="gold" >Lab for HII </span></p>
<br>
<div class="left1">
<span style="font-size:0.8em" >Use the Lab guide and follow the steps<br>Adding HII to the UEFI Driver for the UEFI Driver Wizard Lab</span>
<ul>
  <li> <span style="font-size:0.7em" >link to <a href="https://legacy.gitbook.com/book/laurie0131/uefi_driver_hii_linux_lab_guide/details">PDF Linux</a></span> </li>
  <li> <span style="font-size:0.7em" >link to <a href="https://legacy.gitbook.com/book/laurie0131/uefi_driver_hii_win_lab_guide/details">PDF Windows</a></span> </li>
</ul>
</div>
<div class="right1">
<span style="font-size:0.8em" >&nbsp;  </span>
</div>

Note:

---
@title[Reference]
### <p align="right"><span class="gold" >Reference</span></p>
<br>
<p style="line-height:90%"><span style="font-size:0.9em" >Unified Extensible Firmware Interface Specification, Version 2.7, <a href="http://www.uefi.org">http://www.uefi.org</a> (UEFI 2.1 or greater needed for HII)</span></p>
<br>
<p style="line-height:90%"><span style="font-size:0.9em" >VFR Programming Language 1.92, <a href="https://github.com/tianocore/tianocore.github.io/wiki/EDK-II-Specifications#vfr">EDK-II-Specifications#vfr </a>  </span> </p>
<br>
<p style="line-height:90%"><span style="font-size:0.9em" >Build Spec 1.28,   <a href="https://github.com/tianocore/tianocore.github.io/wiki/EDK-II-Specifications#build">EDK-II-Specifications#build </a> </span> </p>





---  
@title[Summary]
##### <p align="center"<span class="gold"   >Summary </span></p><br>

 @fa[certificate gp-bullet-green]<span style="font-size:0.9em">&nbsp;&nbsp;What is the Infrastructure for HII </span><br><br>
 @fa[certificate gp-bullet-cyan]<span style="font-size:0.9em">&nbsp;&nbsp;How Does HII Work </span><br><br>
 @fa[certificate gp-bullet-yellow]<span style="font-size:0.9em">&nbsp;&nbsp;Lab for HII</span> <br><br>
 

---?image=assets/images/gitpitch-audience.jpg
@title[Questions]
<br>
![Questions](/assets/images/questions.JPG =10x) 


---?image=assets/images/gitpitch-audience.jpg
@title[Logo Slide]
<br><br><br>
![Logo Slide](/assets/images/TianocoreLogo.png =10x)


---
@title[Acknowledgements]
#### <p align="center"><span class="gold"   >Acknowledgements</span></p>

```c++
/**
Redistribution and use in source (original document form) and 'compiled' forms (converted
to PDF, epub, HTML and other formats) with or without modification, are permitted provided
that the following conditions are met:

Redistributions of source code (original document form) must retain the above copyright 
notice, this list of conditions and the following disclaimer as the first lines of this 
file unmodified.

Redistributions in compiled form (transformed to other DTDs, converted to PDF, epub, HTML
and other formats) must reproduce the above copyright notice, this list of conditions and 
the following disclaimer in the documentation and/or other materials provided with the 
distribution.

THIS DOCUMENTATION IS PROVIDED BY TIANOCORE PROJECT "AS IS" AND ANY EXPRESS OR IMPLIED 
WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND 
FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL TIANOCORE PROJECT BE 
LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES 
(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, 
DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, 
WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) 
ARISING IN ANY WAY OUT OF THE USE OF THIS DOCUMENTATION, EVEN IF ADVISED OF THE POSSIBILITY 
OF SUCH DAMAGE.

Copyright (c) 2018, Intel Corporation. All rights reserved.
**/

```
