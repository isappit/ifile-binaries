![Logo](http://www.isapp.it/images/logo/Logo_isapp_it_250x87.png)

# Welcome to the *IFile Binaries* Release!

## RELEASE INFORMATION

*IFile Binaries 2.0dev*

Please see [CHANGELOG.md](CHANGELOG.md).

### What is IFile Binaries?
IFile Binaries is an repository of third-parts binaries files used from IFile to retrieve the content of many type of files.

### Third-parts
IFile for now uses two third-parts binaries files:

#### XPDF
IFile uses the third-part component XPDF to get the content of the PDF files.
[more detail](http://www.foolabs.com/xpdf/)

IFile integrate many version of XPDF for different Operating System (OS):

- Freebsd 32bit
- Linux 32bit and 64bit
- OSX 64bit
- Windows 32bit and 64bit

If you use an different OS, you can install on your server the correct XPDF and configure IFile to use the XPDF installed on your OS, read [README.md](https://github.com/isappit/ifile/blob/master/src/Config/xml/README.md) for correct configuration.

#### ANTIWORD
IFile uses the third-part component ANTIWORD to get the content of the Microsoft Word Document files.
[more detail](http://www.winfield.demon.nl/) 

IFile integrate version of ANTIWORD only:

- Linux 32bit
- Windows 32bit

*IMPORTANT:*

If you use an different OS, you must for now (we hope to integrate the configuration of the absolute path of executable files, in the next release of IFile) copy the executable file compiled on your server, in the correct folder in binaries files.

### How Download and use Binaries files in IFile
If you want use third-part component XPDF or ANTIWORD you need:

 - Download the binaries files from [here](https://github.com/isappit/ifile-binaries/archive/master.zip)
 - Unzip the package on your server
 - Copy the _"ifile-binaries"_ folder in _"vendor/isappit/ifile/src/Adapter/Helpers/"_ or configure IFile to read the "ifile-binaries" folder from external path at IFile. [More detail](https://github.com/isappit/ifile/blob/master/src/Config/xml/README.md) 

 Example how configure external path:
```xml
 <binaries>/usr/local/var/ifile/ifile-binaries</binaries>
```

### LICENSE

For License of every third-parts components see the respective websites:

[ANTIWORD](http://www.winfield.demon.nl/) 

[XPDF](http://www.foolabs.com/xpdf/about.html)