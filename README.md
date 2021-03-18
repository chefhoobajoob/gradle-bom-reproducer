All files named file-1.js and file-2.js include a UTF-8 BOM

All files named file-3.js have no BOM

1. clone repo onto Ubuntu Bionic system
2. run ./gradle distZip
3. extract ./build/distributions/anything.zip
4. note that the first line of every occurrence of file-1.js and file-2.js from the distribution zip has `???` as the leading character sequence, and no BOM
5. note that the sequence `???` does not appear in any file from the distribution named file-3.js
