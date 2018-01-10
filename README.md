# book-template
This is the latex book template of Chinese edition AGT book.

The following is the example of command:

1.`\firstgls{AGT}` will look like this **,算法博弈论（algorithmic game theory）**

2.`\firstacr{AGT}` will look like this **,算法博弈论（AGT）**

3.`\glsacr{AGT}` will look like this 算法博弈论（AGT）

4.`\firstall{AGT}` will look like this **,算法博弈论（algorithmic game theory，AGT）**

5.`\gls{AGT}` will look like this , 算法博弈论。

6.`\glssymbol{AGT}` will look like this AGT。

7.`\glsdesc{AGT}` will look like this algorithmic game theory。

Commands above is used to replace the word which is in the index in the text, and then these pages will appear in the index.

if you use Windows system, then you can go to this site https://tug.org/texlive/acquire-netinstall.html to download the texlive 2017.
just click the 
> install-tl-windows.exe

to download the setup software.

If you use the mac os, just install the MacTex. You can download it at https://tug.org/mactex/

What's more, you are recommanded to use the xelatex command to compile the agt-chinese.tex file to get the pdf file.

If you want to get the index at the last of this book, you can download perl at http://strawberryperl.com/ which is for Windows user, and for mac or linux user the perl environment has been installed in the system. You can follow the steps following to get the index.

You should firstly xelatex the file 
>agt_chinese.tex

. Then use the command line (windows powershell or bash for linux etc.) in the directary "$your path$/agt_chinese" and input the `makeglossaries agt_chinese` .
After the compile, xelatex the >
agt_chinese.tex
again, you can get the index.

If there are some errors like "unknown option for the package `glossaries'" you should update the package to slove it.
