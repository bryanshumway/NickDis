1.Download and install Miktex.
2.Open Miktex Console.(If it doesn't work on the first time might need reset computer.)
3.Open Texworks(icon with T on console)
4.Load the file you wish to edit.
Alternatively you may select the file in the file directory.

To generate pdf select typeset > pdfLaTeX+MakeIndex+BibTeX then press the button with an arrow.

If you wish for text to appear in default paragraph style no format specifiers are needed.(except for certain symbols)
to include % use \%.
to include < use \textless
to include > use \textgreater
to include pi symbol use \pi between $ ($ switches to math mode)
specify seperate paragraphs by leaving an empty line between.

For citations add \cite{(citation name)}
For new entries add a bibtex entry to dis.bib				*current naming convention is first authors last name and year

To add comments start a line with %.					*no midline commenting

Start a file for each chapter. Use \chapter{(chapter name)} to give the chapter a name.
To specify sections use \section{(section name)}
To specify subsections use \subsection{(subsection name)}
To specify subsubsections use \subsubsection{(subsubsection name)}	*lowest order and not included in table of contents

If you are going to include images in a file designate the path as graphicspath{.\images\(source folder)\}
For figures use:
\figure[H]{
   \centering
   \includegraphics[(optional width = \linewidth)]{(source image)}	*linewidth is just recommended for wide images
   \caption{(figure caption)}
}
For tables use above except replace figure with table

For code text use \texttt{(code text)}
For italics use \textit{(italic text)}

Table of contents automatically adds in chapters, sections and subsections.
Table of figures automatically adds in figures.
Table of tables automatically adds in tables.

To add a file insert at the appropriate location in the dis.tex file with \include{file name}.

To allow current tex file(dis.tex is automatic) to create the pdf include the following line at the top:
% !Tex root = dis.tex

pdf may take a couple minutes to load. Currently appendix C cost the most time so commenting it out should improve load time.