# connect
Connect to a computer in AD where the current user is in a the local Admininstrators group  ;on that computer, via domain or local group, or directly.  Use AD computer name. Global $oService = _TS_Open("COMPUTERNAME")  ;Connect to a computer in AD where the entered user (AdminUser) is an AD user, and is in a the  ;local Admininstrators group on that computer, via domain or local group, or directly.  Use AD computer name. Global $oService = _TS_Open("COMPUTERNAME", "AdminUser", "AD", "Password")   ;Connect to a computer in AD where the entered local user (Administrator) is NOT an AD user,  ;and is in a the local Admininstrators group on that computer, via local group, or directly.  Use AD computer name. Global $oService = _TS_Open("COMPUTERNAME", "Administrator", ".", "Password")   ;Non-domain computer where the entered local user (Administrator) is in a the local Admininstrators group  ;on that computer.  Use IP address or DNS name to connect. Global $oService = _TS_Open("192.168.0.1", "Administrator", ".", "Password")
