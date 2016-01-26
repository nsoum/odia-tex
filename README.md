----------------------------------------------------------------------------------
Odia-TeX v0.10                                                     24 January 2016
----------------------------------------------------------------------------------

Copyright (C) 1996-2016 Jeroen Hellingman (JH), Soumyashant Nayak (SN) 
& Anshuman Pandey (AP). 
(in alphabetical order of last name)

This work may be freely used and distributed in the spirit of the LaTeX 
Project Public License (LPPL) and the GNU General Public License (GPL).

Note that the instructions below are for a GNU/Linux system (tested on
Linux Mint 17 Qiana). 

Getting started : 

1. In your system, open the configuration file 
<code>/usr/share/texmf/web2c/texmf.cnf</code> and ensure that the following is 
set, <code>TEXMFHOME = ~/texmf</code> .

2. Create a directory named <code>texmf</code> (if there isn't one) in the home 
folder and create the standard TeX directory structure inside it. In simpler terms,
create sub-directories named <code>bibtex, fonts, metafont, metapost, tex, doc, 
scripts</code> in <code>~/texmf/</code>.

3. In the directory <code>~/texmf/fonts/</code>, create sub-directories <code>gf, 
pk, source, tfm</code>. Copy the folders <code>odia-build-metafont, odia-fonts</code> 
from the repository into <code>~/texmf/fonts/source/</code>.

4. Copy the folder <code>odia-tex-core</code> from the repository into
<code>~/texmf/tex/</code>. 

5. Inform texmf to look into your new local TeX directory structure by 
running the following command in the commandline prompt <code>$ sudo update-texmf</code>
(without the $ sign).

6. At the commandline prompt, run <code>$ tex odmacs.tex</code> (without the $ sign). 
Metafont should generate all the fonts now. This may take a few minutes. At the end of 
the process, type <code>\end</code>.

Now TeX on your system is ready to recognise Odia fonts. For type-setting
tutorials and tips, please refer to the manual <code>odia-tex-manual.pdf</code> in the 
<code>doc</code> folder in the repository.

NOTE : Odia-TeX is a work in progress.<br /><br /> 

Soumyashant Nayak,<br />
nsoum@math.upenn.edu

