# Kira (DICOM-RT-Anonymizer)
Anonymize DICOM-RT files with ease. UIDs are also anonymized without losing RT connections.

![Test Image 6](https://github.com/Kiragroh/Kira_DICOM-RT-Anonymizer-MG/blob/main/GUIscreenshot.PNG)

I build this little tool named Kira because I could not find a sufficient free DICOM-Anonymizer that works great with radiotherapy specific files.
Most anonymizer have one of the following problems:
- RT connection specific UIDs will not be changed -> No import to the original TPS possible
- RT connection specific UIDs get broken -> No import for any TPS possible

I think I was able to solve these problems. :)
In addition, I give the option of changing the linac of RTPLAN files (LinacName, LinacID and ManufacturerModelName). This can be necessary for TPS-Import.

The heavy work is done by EvilDicom (C# package from Rex Cardan: https://github.com/rexcardan/Evil-DICOM). 
I highly recommend it.

A future release will include two additional features:
1.) CyberKnife conversion of RD-files for frequently used TPS (Eclipse and co.).
2.) Automatic generation of RP-Dummy-Plans.

This additional features will make plan comparison study much easier.

![Test Image 6](https://github.com/Kiragroh/Kira_DICOM-RT-Anonymizer-MG/blob/main/Future.PNG)
