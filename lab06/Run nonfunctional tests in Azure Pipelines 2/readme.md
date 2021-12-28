# PROBLEMY
- tym razem problemy są z wget'em i tarball'em w którym jest apache-jmeter
- Azure Pipeline po ściągnięciu (wget), twierdzi, że archiwum _.tgz_ ma błędy:

> _gzip: stdin: not in gzip format_
> _tar: Child returned status 1_
> _tar: Error is not recoverable: exiting now_
> _##[error]Bash exited with code '2'.__

- jednak na lokalnym komputerze (Linux Mint 20.1) polecenia działają OK

> wget http://ftp.ps.pl/pub/apache/jmeter/binaries/apache-jmeter-5.4.1.tgz
> tar -xzf apache-jmeter-5.4.1.tgz

## Uwaga:
- po ponownym uruchomieniu (bez żadnych zmian w repo), pipeline zadziałał OK - co było problemem? - Microsoft wie...