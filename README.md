# LaTeX Thesis Template - ITESM

This a template for ITESM thesis projects in English.

This template was inspired by the [phdDissertationFormat.sty](https://www.overleaf.com/latex/templates/itesm-mit-masterthesis/kbkcbxbhxvwy) file created by Luis Marcelo Fernandez Carrasco. Updated by Daniel Solano (_daster_).

The template uses a LaTeX class file 'TecThesis.cls', and a 'definitions.sty' file.

## Folder structure

```
.
├── Additional                      # FOLDER for additional .tex files
│   ├── abstractFile.tex            # .tex file for the abstract
│   ├── acknowledgementFile.tex     # .tex file for acknowledgements
│   ├── Appendix_01.tex             # .tex file for appendix
│   ├── dedicationFile.tex          # .tex file for the dedication
│   └── vitaFile.tex                # .tex file for your CV
├── Chapters                        # FOLDER for thesis chapters
│   ├── Chapter_01.tex              # Chapter example
│   └── Chapter_02.tex              # Chapter example
├── main.tex                        # Main .tex file
├── definitions.sty                # .sty file for variable document definitions
├── TecThesis.cls                   # LaTeX class file
├── escudo-itesm.png                # TEC logo
├── References.bib                  # Referneces .bib file
└── README.md
```

## Template manual

Keep the _TecThesis.cls_ class file and the _definitions.sty_ style file, in your project folder file, and load them from the main.tex file. DO NOT change the first to arguments of main.tex:

```
\documentclass{TecThesis} 
\usepackage{definitions}
```

Fell free to modify your personal and project information using the _definitions.sty_ file:

```
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%  Author's / DATE / TITLE
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%% The research center you are associated with:
\researchCenter{Research Center}

%%  VERY IMPORTANT: Your name / AUTHOR'S NAME: 
\doctoralStudent{Juanito Perez}

%%  The month when you give your thesis:
\dissertationMonth{April}

%%  The year when you give your thesis:
\dissertationYear{2023}

%%  The title of your dissertation:
\dissertationTitle{Thesis title}

%%  The campus where you are to give your thesis:
\campus{Monterrey}

%%  Your major
\major{Nanotechnology}

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%  Advisor & Commitee members
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%  Your advisor's name:
\advisor{Dr. Advisors Name}

%%  Your advisor's institution:
\advisorInstitution{Tecnol\'{o}gico de Monterrey}

%%  Committee member A's name:
\committeeMemberA{Committee member A's name}

%%  Committee member A's institution:
\committeeMemberAInstitution{Committee member A's institution}

%%  Committee member B's name:
\committeeMemberB{Committee member B's name}

%%  Committee member B's institution:
\committeeMemberBInstitution{Committee member B's institution}

%%  Graduate program director's name:
\graduateProgramDirector{Dr. Jorge Welti Chanes}        			

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%  Load the required files such as Abstract, acknowledgements, det,etc.
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
\abstractFile{./Additional/abstractFile}                                     	%%  This is a plain tex file that holds your abstract
\acknowledgementFile{./Additional/acknowledgementFile}                       	%%  This is a plain tex file that holds your acknowledgements
\dedicationFile{./Additional/dedicationFile}                                 	%%  This is a plain tex file that holds your dedication

```
