<h1>Privilege Escalation</h1>

<h2>📝Notes</h2>
<h4>🐚Sending & receiving shells</h4>
<p>Shell = used when interfacing with CLI (Command Line environments); eg. Linux sh or bash</p>
<ul>
  <li>Reverse shell (receive): force the remote server to send command line access to the server; tools used to set up a listener which would be used to receive the connection; bypass firewall rules that may prevent you from connecting to arbitrary ports on the target</li>
  <li>Bind shell (send): open up a port on the server to connect to in order to execute further commands; may be prevented by firewalls protecting the target </li>
</ul>

<h4>Interactivity:</h4>
<ul>
  <li>Interactive: allows interaction with programs after executing them (eg. Powershell, Bash, sh)</li>
  <img src="https://github.com/inezchong7/Privilege-escalation/assets/106855786/68213e8b-2a82-4281-8225-26872333afdd">
  <li>Non-interactive: limited to using programs which do not require user interaction in order to run properly</li>
  <img src="https://github.com/inezchong7/Privilege-escalation/assets/106855786/122e0c0e-91d0-4364-95d8-fc2430db7a6f">
</ul>


<h4>Tools:</h4>
<ul>
  <li>Netcat: receive reverse shells and connect to remote ports attached to bind shells on a target system; installed in Linux</li>
  <li>Socat: more stable than Netcat but also more difficult syntax</li>
  <li>Metasploit: multi/handler - obtain stable shells + improve them; only way to interact w meterpreter shell; handle staged payloads</li>
  <li>Msfvenom: generate payloads other than reverse and bind shells</li>
</ul>
