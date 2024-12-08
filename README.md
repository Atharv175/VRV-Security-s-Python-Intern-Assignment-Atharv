Log Analysis Project
Overview
This project was developed as part of a company's technical assignment to analyze web server logs using Python. The project goes beyond basic log analysis by incorporating advanced reporting, visualization, and user-friendly output formats.

Key features include parsing server logs to extract valuable insights such as the number of requests per IP address, the most frequently accessed endpoint, and detecting suspicious activities like failed login attempts. Additionally, the project generates polished reports in multiple formats (CSV, HTML, and PowerPoint), making it easy to present the findings to stakeholders.

Core Features
Log Analysis:

Analyze web server logs to extract critical metrics:
Requests per IP Address: Identify the most active IPs accessing the server.
Most Accessed Endpoint: Highlight the resource (URL) that receives the most traffic.
Suspicious Activity Detection: Detect potential brute force login attempts by tracking failed login requests (status code 401).
Multi-Format Reporting:

CSV Report:
A structured tabular report containing all the analyzed data.
HTML Report:
A visually appealing, Bootstrap-styled web report with charts and sortable tables.
PowerPoint Presentation:
A professional slide deck summarizing the analysis, ready for presentations.



Extra Efforts (Beyond Assignment Requirements):

HTML Report Enhancements:
Added charts using Chart.js to visualize requests per IP.
Styled using Bootstrap for a professional look.
Included key metrics in a summary section at the top of the report.
PowerPoint Report:
Automatically generates a slide deck summarizing the analysis, including top IPs, endpoints, and suspicious activity.
Improved Terminal Output:
Clean and organized terminal display for quick insights during execution.
File Structure
bash
Copy code
Log_Analysis_Project/
│
├── log_analysis.py          # Main Python script
├── sample.log               # Input log file for analysis
├── report_template.html     # HTML template for the report
├── log_analysis_results.csv # Generated CSV report
└── log_analysis_report.pptx # Generated PowerPoint presentation


Technologies Used
Python Libraries:
collections.Counter: For efficient counting and analysis of log data.
jinja2: For rendering the HTML report dynamically.
python-pptx: For creating professional PowerPoint presentations.
pandas: For easy data manipulation and formatting.
Bootstrap: To style the HTML report.
Chart.js: For adding interactive charts to the HTML report.



How to Run the Project
Requirements
Python 3.x installed on your machine.
Install the required Python libraries:
bash
Copy code
pip install python-pptx jinja2 pandas
Steps to Run
Place Your Log File:
Add your web server log file (e.g., sample.log) to the project folder.
Run the Script:
Execute the Python script:
bash
Copy code
python log_analysis.py
Outputs:
CSV File: log_analysis_results.csv contains the analyzed data in a tabular format.
HTML Report: log_analysis_report.html is a polished, interactive report for viewing in a browser.
PowerPoint Presentation: log_analysis_report.pptx is a professional slide deck summarizing the key findings.


Example Outputs
Terminal Output:
yaml
Copy code
Requests per IP Address:
203.0.113.5          8
198.51.100.23        8
192.168.1.1          7
10.0.0.2             6
192.168.1.100        5

Most Frequently Accessed Endpoint:
/login (Accessed 13 times)

Suspicious Activity Detected:
No suspicious activity detected.

Results saved to F:\Log_Analysis_Project\log_analysis_results.csv
HTML report generated: F:\Log_Analysis_Project\log_analysis_report.html
PPT generated: F:\Log_Analysis_Project\log_analysis_report.pptx
HTML Report:


PowerPoint Report:

Key Takeaways
Clean and Organized Code:
The script is modular, readable, and adheres to Python best practices.
Real-World Relevance:
The project showcases log analysis techniques that are essential for monitoring and securing web server environments.
Polished Presentation:
The multi-format reports (HTML and PowerPoint) add value for stakeholders by presenting data in an easy-to-digest format.
How We Went Beyond Expectations
Interactive HTML Report: Added charts, sortable tables, and a professional layout to make the report visually engaging.
PowerPoint Generation: Automated the creation of a professional slide deck, a feature that was not part of the original requirements.
Terminal Output: Enhanced readability to provide quick insights directly in the terminal.



Acknowledgments
This project was developed as part of a technical assignment for a reputed company specializing in cybersecurity. It was a valuable opportunity to demonstrate our ability to analyze data and present insights effectively.
