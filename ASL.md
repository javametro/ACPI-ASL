* AML (ACPI Machine Language)
	* RSDP (Root System Description Pointer)
	* RSDT (Root System Description Table)
	* DSDT (Defferentiated System Description Table), This table contains the primary AML code for the system
	* XSDT (Extended System Description Table)
	* FADT (Fiexed ACPI Description Table), this table contains configuration information about the ACPI hardware and pointers to the FACS and DSDT table
	* SSDT (Secondary System Description Table), Contains additional AML code
	* THRM (CPU Thermal)
* AML code is stored in the BIOS, so a BIOS upgrade could change it.


* ASL
	* Scopes
	* Objects
	* Buffer
	* Bin
	* Package
	* Function 
	* String 
	
	
* Website
	* https://acpica.org/downloads
	
* SCI : A system interrupt used by hardware to notify the OS of ACPI events. The SCI is active low, sharable


* Process
	* Write ASL 
	* use ASL.exe to compile ASL file to AML
	* put AML in BIOS
	* OS use AML interpreter to call functions in DSDT
	* Run code defined in the method, send SCI to OS
	* OS push events to Application?