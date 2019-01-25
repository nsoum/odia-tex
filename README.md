----------------------------------------------------------------------------------
Odia-TeX v0.5                                                     26 February 2016
----------------------------------------------------------------------------------

Copyright &copy; 1996-2016 Jeroen Hellingman (JH), Soumyashant Nayak (SN) 
& Anshuman Pandey (AP). 
(in alphabetical order of last name)

This work may be freely used and distributed in the spirit of the LaTeX 
Project Public License (LPPL) and the GNU General Public License (GPL).

Note that the instructions below are for a GNU/Linux system (tested on
Linux Mint 17 Qiana). 

Installing the fonts :
----------------------- 

1. In your system, open the configuration file 
<code>/usr/share/texmf/web2c/texmf.cnf</code> and ensure that the following is 
set, <code>TEXMFHOME = ~/texmf</code> .

2. Create a directory named <code>texmf</code> (if there isn't one) in the home 
folder and create the standard TeX directory structure inside it. In simpler terms,
create sub-directories named <code>bibtex, fonts, metafont, metapost, tex, doc, 
scripts</code> in <code>~/texmf/</code>.

3. In the directory <code>~/texmf/fonts/</code>, create sub-directories <code>gf, 
pk, source, tfm</code>. Copy the folders <code>odia-build-mf-core, odia-fonts-core</code> 
from the repository into <code>~/texmf/fonts/source/</code>.

4. Copy the folder <code>odia-tex-core</code> from the repository into
<code>~/texmf/tex/</code>. 

5. Copy the folder <code>odia-latex-core</code> from the repository into 
<code>~/texmf/tex/latex</code>.

6. Inform texmf to look into your new local TeX directory structure by 
running the following command in the commandline prompt <code>$ sudo update-texmf</code>
(without the $ sign).

7. At the commandline prompt, run <code>$ tex odmacs.tex</code> (without the $ sign). 
Metafont should generate all the fonts now. This may take a few minutes. At the end of 
the process, type <code>\end</code>.

Now TeX on your system is ready to recognise Odia fonts.


Installing od2tex :
-------------------

<code>od2tex</code> (Copyright &copy; 2016, Soumyashant Nayak, distributed under GNU General Public License )
is a Python-based script to convert Odia text transliterated in English to Odia-TeX syntax. The protocols
 for transliteration, which are quite intuitive, are prescribed in the manual <code>odia-tex-manual.pdf</code> 
in the <code>doc</code> folder in the repository. Follow the steps below to install <code>od2tex</code> on 
a GNU/Linux system.

1. Download the tarball <code>od2tex-0.5.tar.gz</code>, which contains the source code for <code>od2tex</code>, from the <code>src</code> 
directory in the repository.

2. Extract the tarball on your system and go to the extracted folder. Run <code>$ sudo python setup.py install</code>
(without the $ sign) in the commandline. 


For type-setting tutorials and tips, please refer to the manual <code>odia-tex-manual.pdf</code> in the 
<code>doc</code> folder in the repository.

NOTE : Odia-TeX is a work in progress.<br /><br /> 

Soumyashant Nayak,<br />
<tt>odia.bhashakosha [at] gmail [dot] com </tt>

