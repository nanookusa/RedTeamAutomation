# RedTeamAutomation
A project to create a port scanning automation interface allowing for the configuration of scans and the displaying of results.

MVP
The application should allow the operator to configure up to (10) distict scans.  Scanning variables should include:
Scan Name, Scan Technique (sS, sP or sV), IP Range, Port Range, Verbosity Level, optional OS detection, results output file and frequency of scan.
Scan configuration can either be be done via the web interface or by editing a configuration file.
The web interface can be a single page and should display the results of each of the configured scans and provide the ability to pause the scanning queue.

Technologies
The backend of the application should be a Node/Express stack.  The NMAP scanner can be interfaced by using a Javascript wrapper such as node-libnmap. https://github.com/jas-/node-libnmap

Stretch Goal 1
Export Scan results into a locally hosted Elasticsearch instance https://www.npmjs.com/package/elasticsearch.  Feed realtime scan information from Elasticsearch.
Create a second page of the application allowing for querying of realtime and historical scan data.

Stretch Goal 2
Allow for the triggering of nmap scripts based off of results from scanning.  https://nmap.org/book/man-nse.html

Stretch Goal 3
ALlow for the triggering of metaspoilt modules as a result of scanning.  https://github.com/rapid7/metasploit-framework/wiki
