<html>
<h1>tftp</h1>
<p>This is a simple tftp server/client that can be used to transfer a file. It also displays information as the transfer takes place, showing you the packet sizes being sent, the ACK receiving, etc. Heavily inspired by Beej's guide to network programming.</p>
<p>Both the client and server are set on port 69 by default, but this may not be accessible to you, so you can change the port (and host) if you need to.</p>
<p>The received file is named "recvfile.txt" so you can see what was sent and it won't replace the file (in case you choose to do it in the same folder, which you can. It's pretty full featured and will try to resend failed packets a certain number of times before it gives up.</p>
<hr>
<h2>Installation</h2>
<pre>make</pre>
<h2>Uninstallation</h2>
<pre>make clean</pre>
<hr>
<h2>Usage</h2>
<h3>Server</h3>
<pre>./server [-p port]</pre>
<h3>Client</h3>
<pre>./client [-p port] [-h hostname] -f <filename></pre>
</html>
