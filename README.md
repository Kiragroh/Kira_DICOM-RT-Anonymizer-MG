# Kira (DICOM-RT-Anonymizer)
Anonymize DICOM-RT files with ease. UIDs are also anonymized without losing RT connections.

![Test Image 6](https://github.com/Kiragroh/Kira_DICOM-RT-Anonymizer-MG/blob/main/GUIscreenshot.png)

I build this little tool named Kira because I could not find a sufficient free DICOM-Anonymizer that works great with radiotherapy specific files.
Most anonymizer have one of the following problems:
- RT connection specific UIDs will not be changed -> No import to the original TPS possible
- RT connection specific UIDs get broken -> No import for any TPS possible

I think I was able to solve these problems. :)
In addition, I give the option of changing the linac of RTPLAN files (LinacName, LinacID and ManufacturerModelName). This can be necessary for TPS-Import of external plans.

The heavy work is done by EvilDicom (C# package from Rex Cardan: https://github.com/rexcardan/Evil-DICOM). 
I highly recommend it.

Requierements:  
1.) Windows operating system  
2.) rund the .exe in the downloaded and then extracted folder  
3.) have 'Microsoft .NET Framework 4.5' installed. Usually, it is automatically installed on a windows machine. On an internet PC, you will be prompted to install. Otherwise download here: https://www.microsoft.com/de-de/download/details.aspx?id=30653)

A future release will include two additional features:
1.) CyberKnife conversion of RD-files for frequently used TPS (Eclipse and co.).
2.) Automatic generation of RP-Dummy-Plans.

This additional features will make plan comparison studies much easier.

![Test Image 6](https://github.com/Kiragroh/Kira_DICOM-RT-Anonymizer-MG/blob/main/Future.PNG)

Note:
- script is optimized to work with Eclipse 15.1
- absolute ESAPI-beginner should first look at my GettingStartedMaterial (collection of many helpful stuff from me or others and even includes a PDF version of some ESAPI-OnlineHelps)
https://drive.google.com/drive/folders/1-aYUOIfyvAUKtBg9TgEETiz4SYPonDOO
