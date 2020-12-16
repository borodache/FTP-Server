# FTP-Server
FTP Java Server project

how to run:
create runServer.bat in project root directory with content

pushd %~dp0
if not exist Job md Job
@rem copy Job\*.* C:\Users\Eli\Desktop\Job

java -cp bin -Dftp.tracer=util.GuiTracer server.FTPParallelServer

send file for test with windows FTP client
ftp localhost
user/password
put somefile.txt
