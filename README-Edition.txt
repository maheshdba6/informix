Informix edition installer:

You may run the Informix edition installer to switch the edition of a 14.10 Informix installation from one edition to another.

Run the edition installer as the user informix, or as the same user that installed a private installation.


This requires Java 1.8.0 to install.

Launch interactive install using:

[UNIX/Linux]
	$INFORMIXDIR/jvm/jre/bin/java -jar ee_edition.jar -i <console|gui>
[Windows]
	%INFORMIXDIR%\jvm\jre\bin\java.exe -jar ee_edition.jar -i <console|gui>

Silent install can be done with:

[UNIX/Linux]
	$INFORMIXDIR/jvm/jre/bin/java -jar ee_edition.jar -DUSER_INSTALL_DIR=$INFORMIXDIR -DLICENSE_ACCEPTED=TRUE -i silent
[Windows]
	%INFORMIXDIR%\jvm\jre\bin\java.exe -jar ee_edition.jar -DUSER_INSTALL_DIR=%INFORMIXDIR% -DLICENSE_ACCEPTED=TRUE -i silent


Alternatively the ids_install or iwa_install installer will invoke the edition installer for you.  All you need to do is copy ee_edition.jar to the same directory as ids_install, and run the ids_install as normal.

If there are multiple edition installers in the installation folder the first found from the list below will be installed,
	 Advanced Enterprise Edition (aee)
	 Advanced Workgroup Edition (awe)
	 Advanced Developer Edition (ade)
	 Advanced Enterprise Time Limited Edition (aetl)
	 Enterprise Edition (ee)
	 Time Limited Edition (tl)
	 Workgroup Edition (we)
	 Express Edition (e)
	 Innovator-C Edition (ie)
	 Developer Edition (de)
