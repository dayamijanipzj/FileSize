# FileSize
rocedure.s GetIpToHostname(hostname.s)     Define result.s = "", netid.i, ip.l ; Wrong, see below. Procedure.s GetIpToHostname(hostname.s)     Protected result.s = "", netid.i, ip.l Procedure.s FileGetTime (NomFichier.s,flag,DateFormat.s="%mm/%dd/%yyyy %hh:%ii:%ss")     Protected Directory$, FileName$, Time Procedure.s Ping (hostname.s)     Protected Ping, cont, work, risposta.s, time.s Procedure.s FileGetSize(NomFichier.s) ; Update Function     Protected Directory$, FileName$, Size$      FileName$ = NomFichier  ; ???? Procedure.s FileGetSize(NomFichier.s) Procedure.s FileGetSize(FileName$) ; Directly variable  Macro FileGetSize(FileName)     FileSize(FileName) EndMacro  Debug FileGetSize ( "C:\Windows\explorer.exe" )
