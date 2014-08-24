Reagan-
=======
5	5	 # File(s) to watch
6	6	 watch /var/log/auth.log
7	+watch /var/log/secure.log
7	8	 
8	9	 # Logfile patterns look out for
9	10	 address 'Invalid user [^[:space:]]+ from ([^[:space:]]+)' 1
10	11	 address 'Failed password for [^[:space:]]+ from ([^[:space:]]+)' 1
11	12	 address 'Failed password for invalid user [^[:space:]]+ from ([^[:space:]]+)' 1
13	+address 'Failed keyboard-interactive/pam for invalid user [^[:space:]]+ from ([^[:space:]]+)' 1
12	14	 
13	15	 # Address patterns to exempt
14	16	 exempt 127.0.0.1
