# netstat_logging-via-powershell
A very simple pair of scripts using powershell to query netstat and output the timestamped results to a file. Can be simply executed from Windows Task Scheduler using the batch file. Does not require modification of ExecutionPolicy.

Keep both scripts within the same directory. Logs will be output to a file `logs.txt` within the same directory. Users can move the directory anywhere or rename it so long as the files are kept together.

When either the .bat or .ps1 is run from the command line, the powershell window is kept open pending a user keystroke so that users can view any errors.

This script is primarily made available as an example of the following Powershell concepts: 

	- Executing a Powershell script via a batcsh file 
	- Allowing the execution of unsigned Powershell scripts without permanent changes to ExecutionPolicy
	- Parsing heightened user privelegs to Powershell scripts	
	
While these concepts are not complex, they are counterintuitive for users familiar with using the Bourne shell command syntax in operating systems that do not have similar hoops to jump through. Furthermore, `netstat` can easily be replaced with more complex and relevant commands.

As time permits, I will add support for command line parameters like modifying the path of logging.