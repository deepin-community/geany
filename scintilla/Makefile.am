
SUBDIRS = include

noinst_LTLIBRARIES=libscintilla.la

AM_CXXFLAGS = -DNDEBUG -DGTK -DSCI_LEXER -DNO_CXX11_REGEX

LEXER_SRCS= \
lexers/LexAbaqus.cxx \
lexers/LexAda.cxx \
lexers/LexAsm.cxx \
lexers/LexBash.cxx \
lexers/LexBasic.cxx \
lexers/LexBatch.cxx \
lexers/LexCOBOL.cxx \
lexers/LexCPP.cxx \
lexers/LexCSS.cxx \
lexers/LexCaml.cxx \
lexers/LexCmake.cxx \
lexers/LexCoffeeScript.cxx \
lexers/LexD.cxx \
lexers/LexDiff.cxx \
lexers/LexErlang.cxx \
lexers/LexForth.cxx \
lexers/LexFortran.cxx \
lexers/LexHTML.cxx \
lexers/LexHaskell.cxx \
lexers/LexJulia.cxx \
lexers/LexLaTeX.cxx \
lexers/LexLisp.cxx \
lexers/LexLua.cxx \
lexers/LexMake.cxx \
lexers/LexMarkdown.cxx \
lexers/LexMatlab.cxx \
lexers/LexNsis.cxx \
lexers/LexNull.cxx \
lexers/LexPascal.cxx \
lexers/LexPerl.cxx \
lexers/LexPowerShell.cxx \
lexers/LexProps.cxx \
lexers/LexPython.cxx \
lexers/LexPO.cxx \
lexers/LexR.cxx \
lexers/LexRuby.cxx \
lexers/LexRust.cxx \
lexers/LexSmalltalk.cxx \
lexers/LexSQL.cxx \
lexers/LexTCL.cxx \
lexers/LexTxt2tags.cxx \
lexers/LexVHDL.cxx \
lexers/LexVerilog.cxx \
lexers/LexYAML.cxx

SRCS= \
gtk/Converter.h \
gtk/PlatGTK.cxx \
gtk/ScintillaGTK.cxx \
gtk/ScintillaGTK.h \
gtk/ScintillaGTKAccessible.cxx \
gtk/ScintillaGTKAccessible.h \
gtk/scintilla-marshal.c \
gtk/scintilla-marshal.h \
lexlib/Accessor.cxx \
lexlib/Accessor.h \
lexlib/CatalogueModules.h \
lexlib/CharacterCategory.cxx \
lexlib/CharacterCategory.h \
lexlib/CharacterSet.cxx \
lexlib/CharacterSet.h \
lexlib/DefaultLexer.cxx \
lexlib/DefaultLexer.h \
lexlib/LexAccessor.h \
lexlib/LexerBase.cxx \
lexlib/LexerBase.h \
lexlib/LexerModule.cxx \
lexlib/LexerModule.h \
lexlib/LexerNoExceptions.cxx \
lexlib/LexerNoExceptions.h \
lexlib/LexerSimple.cxx \
lexlib/LexerSimple.h \
lexlib/OptionSet.h \
lexlib/PropSetSimple.cxx \
lexlib/PropSetSimple.h \
lexlib/SparseState.h \
lexlib/StringCopy.h \
lexlib/StyleContext.cxx \
lexlib/StyleContext.h \
lexlib/SubStyles.h \
lexlib/WordList.cxx \
lexlib/WordList.h \
src/AutoComplete.cxx \
src/AutoComplete.h \
src/CallTip.cxx \
src/CallTip.h \
src/CaseConvert.cxx \
src/CaseConvert.h \
src/CaseFolder.cxx \
src/CaseFolder.h \
src/Catalogue.cxx \
src/Catalogue.h \
src/CellBuffer.cxx \
src/CellBuffer.h \
src/CharClassify.cxx \
src/CharClassify.h \
src/ContractionState.cxx \
src/ContractionState.h \
src/DBCS.cxx \
src/DBCS.h \
src/Decoration.cxx \
src/Decoration.h \
src/Document.cxx \
src/Document.h \
src/Editor.cxx \
src/Editor.h \
src/EditModel.cxx \
src/EditModel.h \
src/EditView.cxx \
src/EditView.h \
src/ElapsedPeriod.h \
src/ExternalLexer.cxx \
src/ExternalLexer.h \
src/FontQuality.h \
src/Indicator.cxx \
src/Indicator.h \
src/IntegerRectangle.h \
src/KeyMap.cxx \
src/KeyMap.h \
src/LineMarker.cxx \
src/LineMarker.h \
src/MarginView.cxx \
src/MarginView.h \
src/Partitioning.h \
src/PerLine.cxx \
src/PerLine.h \
src/Position.h \
src/PositionCache.cxx \
src/PositionCache.h \
src/RESearch.cxx \
src/RESearch.h \
src/RunStyles.cxx \
src/RunStyles.h \
src/SVector.h \
src/ScintillaBase.cxx \
src/ScintillaBase.h \
src/Selection.cxx \
src/Selection.h \
src/SparseVector.h \
src/SplitVector.h \
src/Style.cxx \
src/Style.h \
src/UniConversion.cxx \
src/UniConversion.h \
src/UnicodeFromUTF8.h \
src/UniqueString.cxx \
src/UniqueString.h \
src/ViewStyle.cxx \
src/ViewStyle.h \
src/XPM.cxx \
src/XPM.h \
$(LEXER_SRCS)

libscintilla_la_SOURCES = $(SRCS)

AM_CPPFLAGS = -I$(top_srcdir) -I$(srcdir)/include -I$(srcdir)/src -I$(srcdir)/lexlib \
	@GTK_CFLAGS@ @LIBGEANY_CFLAGS@

marshallers: gtk/scintilla-marshal.list
	glib-genmarshal --prefix scintilla_marshal gtk/scintilla-marshal.list --header > gtk/scintilla-marshal.h
	glib-genmarshal --prefix scintilla_marshal gtk/scintilla-marshal.list --body > gtk/scintilla-marshal.c

EXTRA_DIST=gtk/scintilla-marshal.list License.txt README version.txt
