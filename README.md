---
author:
- The MIT License (MIT)
title: "-----------------------------------------------------------------------------------------------------------------------------------------------%"
---

\% Copyright (c) 2021 Jitin Nair % % Permission is hereby granted, free
of charge, to any person obtaining a copy % of this software and
associated documentation files (the "Software"), to deal % in the
Software without restriction, including without limitation the rights %
to use, copy, modify, merge, publish, distribute, sublicense, and/or
sell % copies of the Software, and to permit persons to whom the
Software is % furnished to do so, subject to the following conditions:
%\
% THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR % IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, % FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE % AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER % LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, % OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN % THE SOFTWARE. %\
%
%-----------------------------------------------------------------------------------------------------------------------------------------------%

%----------------------------------------------------------------------------------------
% DOCUMENT DEFINITION
%----------------------------------------------------------------------------------------

\% article class because we want to fully customize the page and not use
a cv template
```{=tex}
\documentclass[a4paper,11pt]{article}

%----------------------------------------------------------------------------------------
%   FONT
%----------------------------------------------------------------------------------------

% % fontspec allows you to use TTF/OTF fonts directly
% \usepackage{fontspec}
% \defaultfontfeatures{Ligatures=TeX}

% % modified for ShareLaTeX use
% \setmainfont[
% SmallCapsFont = Fontin-SmallCaps.otf,
% BoldFont = Fontin-Bold.otf,
% ItalicFont = Fontin-Italic.otf
% ]
% {Fontin.otf}

%----------------------------------------------------------------------------------------
%   PACKAGES
%----------------------------------------------------------------------------------------
\usepackage{url}
\usepackage{parskip}    

%other packages for formatting
\RequirePackage{color}
\RequirePackage{graphicx}
\usepackage[usenames,dvipsnames]{xcolor}
\usepackage[scale=0.9]{geometry}

%tabularx environment
\usepackage{tabularx}

%for lists within experience section
\usepackage{enumitem}

% centered version of 'X' col. type
\newcolumntype{C}{>{\centering\arraybackslash}X} 

%to prevent spillover of tabular into next pages
\usepackage{supertabular}
\usepackage{tabularx}
\newlength{\fullcollw}
\setlength{\fullcollw}{0.47\textwidth}

%custom \section
\usepackage{titlesec}               
\usepackage{multicol}
\usepackage{multirow}

%CV Sections inspired by: 
%http://stefano.italians.nl/archives/26
\titleformat{\section}{\Medium\scshape\raggedright}{}{0em}{}[\titlerule]
\titlespacing{\section}{0pt}{10pt}{10pt}

%for publications
\usepackage[style=authoryear,sorting=ynt, maxbibnames=2]{biblatex}

%Setup hyperref package, and colours for links
\usepackage[unicode, draft=false]{hyperref}
\definecolor{linkcolour}{rgb}{0,0.2,0.6}
\hypersetup{colorlinks,breaklinks,urlcolor=linkcolour,linkcolor=linkcolour}
\addbibresource{citations.bib}
\setlength\bibitemsep{1em}

%for social icons
\usepackage{fontawesome5}

%debug page outer frames
%\usepackage{showframe}

%----------------------------------------------------------------------------------------
%   BEGIN DOCUMENT
%----------------------------------------------------------------------------------------
\begin{document}

% non-numbered pages
\pagestyle{empty} 

%----------------------------------------------------------------------------------------
%   TITLE
%----------------------------------------------------------------------------------------

% \begin{tabularx}{\linewidth}{ @{}X X@{} }
% \huge{Your Name}\vspace{2pt} & \hfill \emoji{incoming-envelope} email@email.com \\
% \raisebox{-0.05\height}\faGithub\ username \ | \
% \raisebox{-0.00\height}\faLinkedin\ username \ | \ \raisebox{-0.05\height}\faGlobe \ mysite.com  & \hfill \emoji{calling} number
% \end{tabularx}

\begin{tabularx}{\linewidth}{@{} C @{}}
\Huge{Katie Christensen} \\[7.5pt]
{\raisebox{-0.05\height} \ 3319 187th PL SE Bothell, WA 98012} \\ \\
\href{https://github.com/katiechristensen}{\raisebox{-0.05\height}\faGithub\ katiechristensen} \ $|$ \ 
\href{https://linkedin.com/in/katie-r-christensen}{\raisebox{-0.05\height}\faLinkedin\ katie-r-christensen} \ $|$ \ 
\href{mailto:chris90@wwu.edu}{\raisebox{-0.05\height}\faEnvelope \ chris90@wwu.edu} \ $|$ \ 
\href{tel:+14252995511}{\raisebox{-0.05\height}\faPhone \ 425-299-5511} \\
\end{tabularx}

%----------------------------------------------------------------------------------------
%   SUMMARY
%----------------------------------------------------------------------------------------
%Interests/ Keywords/ Summary
%\section{Summary}
%Few sentence summary of me here.

%----------------------------------------------------------------------------------------
%   EDUCATION
%----------------------------------------------------------------------------------------
\section{Education}

\begin{tabularx}{\linewidth}{ @{}l r@{} }
\textbf{Western Washington University} & \hfill Bellingham, WA \\[3.75pt]
Bachelor of Science in Computer Science, 3.41 & \hfill Jun 2023 \\[3.75pt]
\multicolumn{2}{@{}X@{}}{Minor in Biology}  \\
\multicolumn{2}{@{}X@{}}{President's List: Winter 2020, Fall 2020}  \\
\end{tabularx}

%----------------------------------------------------------------------------------------
% EXPERIENCE SECTIONS
%----------------------------------------------------------------------------------------

%Experience
\section{Experience}

\begin{tabularx}{\linewidth}{ @{}l r@{} }
\textbf{HutchResearch} & \hfill Bellingham, WA \\[3.75pt]
\textbf{Undergraduate Research Assistant} & \hfill Sep 2022 - Present \\[3.75pt]

\multicolumn{2}{@{}X@{}}{Currently working on a machine learning (deep learning) project for earth system modeling, specifically predicting climate weather patterns using diffusion models.}  \\
\end{tabularx}

\begin{tabularx}{\linewidth}{ @{}l r@{} }
\textbf{Institute for Systems Biology} & \hfill Seattle, WA \\[3.75pt]
\textbf{Undergraduate Intern Trainee} & \hfill Jun 2022 - Sep 2022 \\[3.75pt]

\multicolumn{2}{@{}X@{}}{Development of a graph-based application programming interface designed to expose knowledge graphs and promote innovative analyses of biomedical questions. The source code and full documentation can be found at https://github.com/gloriachin/KG\_API.}  \\
\end{tabularx}


%----------------------------------------------------------------------------------------
% LEADERSHIP SECTIONS
%----------------------------------------------------------------------------------------

%Leadership
\section{Leadership \& Activities}

\begin{tabularx}{\linewidth}{ @{}l r@{} }
\textbf{Computer Science Mentoring Program} & \hfill Bellingham, WA \\[3.75pt]
\textbf{Administrative Team + Active Mentor} & \hfill Sep 2021 - Present \\[3.75pt]

\multicolumn{2}{@{}X@{}}{The CS Mentoring Program at Western Washington University cultivates supportive and inclusive mentoring relationships with declared CS students and undeclared students interested in pursuing any major in the CS Department. Provide mentor/mentee pairs with training and support to facilitate professional development and foster a positive growth experience for all.}  \\
\end{tabularx}

\begin{tabularx}{\linewidth}{ @{}l r@{} }
\textbf{Association for Gender Inclusion in Computing (AGIC)} & \hfill Bellingham, WA \\[3.75pt]
\textbf{Outreach Coordinator + Active Member} & \hfill Sep 2019 - Present \\[3.75pt]

\multicolumn{2}{@{}X@{}}{Computer Science Department club at Western Washington University.}  \\
\end{tabularx}

\begin{tabularx}{\linewidth}{ @{}l r@{} }
\textbf{Society for Women Engineers (SWE)} & \hfill Bellingham, WA \\[3.75pt]
\textbf{Active Member} & \hfill Sep 2022 - Present \\[3.75pt]

\multicolumn{2}{@{}X@{}}{Engineering Department club at Western Washington University.}  \\
\end{tabularx}

\begin{tabularx}{\linewidth}{ @{}l r@{} }
\textbf{Whatcom Community College Women's Soccer} & \hfill Bellingham, WA \\[3.75pt]
\textbf{Student-Athlete} & \hfill Sep 2020 - Jun 2021 \\[3.75pt]

\multicolumn{2}{@{}X@{}}{NWAC student-athlete for Whatcom Community College women's soccer team.}  \\
\end{tabularx}

%----------------------------------------------------------------------------------------
%   PUBLICATIONS
%----------------------------------------------------------------------------------------
\section{Publications}
\begin{refsection}[citations.bib]
\nocite{*}
\printbibliography[heading=none]
\end{refsection}

%----------------------------------------------------------------------------------------
%   SKILLS
%----------------------------------------------------------------------------------------
\section{Skills}
%\begin{tabularx}{\linewidth}{@{}l X@{}}
%Some Skills &  \normalsize{This, That, Some of this and that etc.}\\
%Some More Skills  &  \normalsize{Also some more of this, Some more that, And some of this and that etc.}\\  
%\end{tabularx}

\begin{tabularx}{\linewidth}{@{}l X@{}}
Python $\>$ $\>$ Java $\>$ $\>$ C $\>$ $\>$ SQL $\>$ $\>$ MySQL $\>$ $\>$ Cypher $\>$ $\>$ Neo4j $\>$ $\>$ FastAPI $\>$ $\>$ DBMS $\>$ $\>$ LaTeX $\>$ $\>$ HTML5 \\
\end{tabularx}

\vfill
\center{\footnotesize Last updated: \today}

\end{document}
```
\\end{document}
