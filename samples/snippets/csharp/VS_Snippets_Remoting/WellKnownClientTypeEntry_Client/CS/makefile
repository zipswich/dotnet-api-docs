all: WellKnownClientTypeEntry_Server.exe WellKnownClientTypeEntry_Client.exe

WellKnownClientTypeEntry_Server.exe: WellKnownClientTypeEntry_Server.cs WellKnownClientTypeEntry_Share.dll
	csc WellKnownClientTypeEntry_Server.cs /r:WellKnownClientTypeEntry_Share.dll

WellKnownClientTypeEntry_Client.exe: WellKnownClientTypeEntry_Client.cs WellKnownClientTypeEntry_Share.dll
	csc WellKnownClientTypeEntry_Client.cs /r:WellKnownClientTypeEntry_Share.dll

WellKnownClientTypeEntry_Share.dll: WellKnownClientTypeEntry_Share.cs
	csc /t:library WellKnownClientTypeEntry_Share.cs
