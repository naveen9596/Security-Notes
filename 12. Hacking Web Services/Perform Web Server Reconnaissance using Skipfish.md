- Skipfish is an active web application (deployed on a webserver) security reconnaissance tool. It prepares an interactive sitemap for the targeted site by carrying out a recursive crawl and dictionary-based probes. The resulting map is then annotated with the output from a number of active (but hopefully non-disruptive) security checks. The final report generated by the tool is meant to serve as a foundation for professional web application security assessments.
- Open Terminal
	> sudo su
	> cd
	
	- Now, perform security reconnaissance on a web server using Skipfish. The target is the WordPress website **http://[IP Address of Windows Server 2016]**.
	- Specify the output directory and load a dictionary file based on the web server’s requirement. In this lab, we are naming the output directory **test**.
	> skipfish -o /root/test -S /usr/share/skipfish/dictionaries/complete.wl http:// #targetip:8080
	
	- On receiving this command, Skipfish performs a heavy **brute-force attack** on the web server by using the **complete.wl** dictionary file, creates a directory named **test** in the **root** location, and stores the result in **index.html** inside this location.
	- Before beginning a scan, Skipfish displays some tips. Press **Enter** to start the security reconnaissance.
	- On completion of the scan, Skipfish generates a report and stores it in the **test** directory (in the **root** location).
	- Expand each node to view detailed information regarding the result.
	- Analyze an issue found in the web server. To do this, click a node under the **Issue type overview** section to expand it.
	- Examine other vulnerabilities and patch them to secure the web server.