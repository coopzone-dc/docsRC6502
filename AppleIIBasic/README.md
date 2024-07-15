This is a ROM Image and a MON txt file, the ROM image conatins WozMon and a CUt-down version of Apple II basic

You can run it with E000R

The txt file is the same apple II basic, as a pastable text MON file. It runs from address 6000H in RAM (6000R)

The original version came from:

https://cowgod.org/replica1/applesoft/

This is a description from the site, note this version does not contain the extra software for the SD-Card/cassette board.

Applesoft Lite: Applesoft BASIC for the Replica-1
Applesoft Lite is a modified version of Applesoft BASIC from the Apple II, designed to run on the Replica-1.

The modifications were made by disassembing the Applesoft ROMs from an Apple II+ and using the S-C DocuMentor as a guide.
Apple II specific things (like graphics) have been removed, and a few Apple-1/Replica-1 specific things have been added.

Supported tokens:
FOR/NEXT, DATA/READ/RESTORE, INPUT, DIM, CALL, HIMEM/LOMEM, ONERR/RESUME, LET, GOTO, RUN/STOP/CONT, IF/THEN
GOSUB/RETURN/POP, END, REM, ON, POKE, PRINT (or "?"), LIST, CLEAR, GET, NEW, TO, SPC, NOT, STEP, +, -, *, /, ^, AND
OR, >, =, <, SGN, INT, ABS, FRE, SQR, RND, LOG, EXP, PEEK, LEN, STR$, VAL, ASC, CHR$, LEFT$, RIGHT$, MID$

Unsupported tokens:
Graphics: TEXT, GR, HGR, HGR2, PLOT, SCRN, HLIN, VLIN, COLOR=, HPLOT, DRAW, XDRAW, HCOLOR=, ROT=, SCALE=
Cassette I/O: STORE, RECALL, SHLOAD (*See also LOAD and SAVE, below)
Text Stuff: HOME, HTAB, VTAB, POS, TAB, NORMAL, FLASH, INVERSE, SPEED=
Math Stuff: COS, SIN, TAN, ATN
Other: DEL, TRACE, NOTRACE, PR#, IN#, WAIT, DEF/FN, USR, & (ampersand), PDL

Notes:
Tokenized Applesoft files from an Apple II will not work, nor will Applesoft Lite files work on an Apple II.
If you'd like to try and load an Apple II program, use the source listing rather than a SAVEd file. Unsupported tokens will result in syntax errors.

Tokenized Integer files will not work either, but the source code may work to some degree.

For the LOAD and SAVE commands, filenames containing BASIC token names are parsed incorrectly, resulting in an error.
For example, you can't 'SAVE PRINT'. This should be fixed in a future release.

The RAM version requires 32K of RAM ($0000-$7FFF), and the ROM version requires 8KB of ROM ($E000-$FFFF).

