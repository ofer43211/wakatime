
History
-------


4.0.15 (2015-06-11)
++++++++++++++++++

- guess language using multiple methods, then use most accurate guess
- use entity and type for new heartbeats api resource schema


4.0.14 (2015-05-31)
++++++++++++++++++

- correctly log message from py.warnings module


4.0.13 (2015-05-16)
++++++++++++++++++

- fix bug with auto detecting project name


4.0.12 (2015-05-15)
++++++++++++++++++

- correctly display caller and lineno in log file when debug is true
- project passed with --project argument will always be used
- new --alternate-project argument


4.0.11 (2015-05-12)
++++++++++++++++++

- reuse SSL connection across multiple processes for improved performance


4.0.10 (2015-05-06)
++++++++++++++++++

- new --cursorpos argument for passing index of cursor within the file contents


4.0.9 (2015-05-06)
++++++++++++++++++

- new --lineno argument for passing line number of cursor at time of heartbeat
- format py.warnings log messages same as other log messages
- include package namespace and line number in logger output


4.0.8 (2015-04-04)
++++++++++++++++++

- added api_url config option and --apiurl cli argument for customizing api url


4.0.7 (2015-04-02)
++++++++++++++++++

- capture warnings in log file


4.0.6 (2015-03-31)
++++++++++++++++++

- add requests.packages directory to sys.path


4.0.5 (2015-03-31)
++++++++++++++++++

- update requests package to v2.0.6
- update simplejson to v3.6.5


4.0.4 (2015-03-09)
++++++++++++++++++

- add back --ignore argument for backwards compatibility


4.0.3 (2015-03-09)
++++++++++++++++++

- refactor module structure


4.0.2 (2015-03-07)
++++++++++++++++++

- include cacert.pem file in pypi distribution for SSL with requests package


4.0.1 (2015-03-03)
++++++++++++++++++

- upgrade requests library to v2.5.3 to fix SSL problem on CentOS
- new options for excluding and including directories


4.0.0 (2015-02-12)
++++++++++++++++++

- use requests library instead of urllib2, so api SSL cert is verified
- new --notfile argument to support logging time without a real file
- new --proxy argument for https proxy support


3.0.5 (2015-01-13)
++++++++++++++++++

- ignore errors from malformed markup (too many closing tags)


3.0.4 (2015-01-06)
++++++++++++++++++

- remove unused dependency, which is missing in some python environments


3.0.3 (2014-12-25)
++++++++++++++++++

- detect JavaScript frameworks from script tags in Html template files


3.0.2 (2014-12-25)
++++++++++++++++++

- detect frameworks from JavaScript and JSON files


3.0.1 (2014-12-23)
++++++++++++++++++

- handle unknown language when parsing dependencies


3.0.0 (2014-12-23)
++++++++++++++++++

- detect libraries and frameworks for C++, Java, .NET, PHP, and Python files


2.1.11 (2014-12-22)
+++++++++++++++++++

- fix offline logging when response from api is None


2.1.10 (2014-12-15)
+++++++++++++++++++

- prevent queuing offline heartbeats which will never be valid (400 errors)


2.1.9 (2014-12-05)
++++++++++++++++++

- fix bug preventing offline heartbeats from being purged after uploaded


2.1.8 (2014-12-04)
++++++++++++++++++

- fix UnicodeDecodeError when building user agent string
- handle case where response is None


2.1.7 (2014-11-30)
++++++++++++++++++

- upgrade pygments to v2.0.1
- always log an error when api key is incorrect


2.1.6 (2014-11-18)
++++++++++++++++++

- fix list index error when detecting subversion project


2.1.5 (2014-11-17)
++++++++++++++++++

- catch exceptions when getting current machine time zone


2.1.4 (2014-11-12)
++++++++++++++++++

- when Python was not compiled with https support, log an error to the log file


2.1.3 (2014-11-10)
++++++++++++++++++

- correctly detect branch name for subversion projects


2.1.2 (2014-10-07)
++++++++++++++++++

- still log heartbeat when something goes wrong while reading num lines in file


2.1.1 (2014-09-30)
++++++++++++++++++

- fix bug where binary file opened as utf-8


2.1.0 (2014-09-30)
++++++++++++++++++

- python3 compatibility changes


2.0.8 (2014-08-29)
++++++++++++++++++

- supress output from svn command


2.0.7 (2014-08-27)
++++++++++++++++++

- find svn binary location from common install directories


2.0.6 (2014-08-07)
++++++++++++++++++

- encode json data as str when passing to urllib


2.0.5 (2014-07-25)
++++++++++++++++++

- option in .wakatime.cfg to obfuscate file names


2.0.4 (2014-07-25)
++++++++++++++++++

- use unique logger namespace to prevent collisions in shared plugin environments


2.0.3 (2014-06-18)
++++++++++++++++++

- use project from command line arg when no revision control project is found


2.0.2 (2014-06-09)
++++++++++++++++++

- include python3.2 compatible versions of simplejson, pytz, and tzlocal
- disable offline logging when Python was not compiled with sqlite3 module


2.0.1 (2014-05-26)
++++++++++++++++++

- fix bug in queue preventing actions with NULL values from being purged


2.0.0 (2014-05-25)
++++++++++++++++++

- offline time logging using sqlite3 to queue editor events


1.0.2 (2014-05-06)
++++++++++++++++++

- ability to set project from command line argument


1.0.1 (2014-03-05)
++++++++++++++++++

- use new domain name wakatime.com


1.0.0 (2014-02-05)
++++++++++++++++++

- detect project name and branch name from mercurial revision control


0.5.3 (2014-01-15)
++++++++++++++++++

- bug fix for unicode in Python3


0.5.2 (2014-01-14)
++++++++++++++++++

- minor bug fix for Subversion on non-English systems


0.5.1 (2013-12-13)
++++++++++++++++++

- second line in .wakatime-project file now sets branch name


0.5.0 (2013-12-13)
++++++++++++++++++

- Convert ~/.wakatime.conf to ~/.wakatime.cfg and use configparser format
- new [projectmap] section in cfg file for naming projects based on folders


0.4.10 (2013-11-13)
+++++++++++++++++++

- Placing .wakatime-project file in a folder will read the project's name from that file


0.4.9 (2013-10-27)
++++++++++++++++++

- New config for ignoring files from regular expressions
- Parse more options from config file (verbose, logfile, ignore)


0.4.8 (2013-10-13)
++++++++++++++++++

- Read git HEAD file to find current branch instead of running git command line


0.4.7 (2013-09-30)
++++++++++++++++++

- Sending local olson timezone string in api request


0.4.6 (2013-09-22)
++++++++++++++++++

- Sending total lines in file and language name to api


0.4.5 (2013-09-07)
++++++++++++++++++

- Fixed relative import error by adding packages directory to sys path


0.4.4 (2013-09-06)
++++++++++++++++++

- Using urllib2 again because of intermittent problems sending json with requests library


0.4.3 (2013-09-04)
++++++++++++++++++

- Encoding json as utf-8 before making request


0.4.2 (2013-09-04)
++++++++++++++++++

- Using requests package v1.2.3 from pypi


0.4.1 (2013-08-25)
++++++++++++++++++

- Fix bug causing requests library to omit POST content


0.4.0 (2013-08-15)
++++++++++++++++++

- Sending single branch instead of multiple tags


0.3.1 (2013-08-08)
++++++++++++++++++

- Using requests module instead of urllib2 to verify SSL certs


0.3.0 (2013-08-08)
++++++++++++++++++

- Allow importing directly from Python plugins


0.1.1 (2013-07-07)
++++++++++++++++++

- Refactored
- Simplified action events schema


0.0.1 (2013-07-05)
++++++++++++++++++

- Birth

