SVN Backups
===========

A Python script for creating full or incremental SVN dumps and uploading the result to Dropbox.  This combines the [Apache SVN backup script](http://svn.apache.org/repos/asf/subversion/trunk/tools/server-side/svn-backup-dumps.py) with the [Python Dropbox Uploader](https://github.com/jncraton/PythonDropboxUploader).  For example, the following command will generate an incremental dump (`-i`), gzip the result (`-z`), and securely upload the resulting backup to Dropbox (`-t dropbox::username:password:/folder`). 

    python svn-backup-dumps.py -z -i -t dropbox::username:password:/folder "C:\SVN\data\repositories\MySVNRepo" .
    
The last two arguments specify the repository location and the local directory where the backups are created.  For incremental backups, do not delete the local backups as this script scans the existing backups to determine the last saved revision.
    
    
Other Open Source Libraries
---------------------------
  - [MOEA Framework](http://www.moeaframework.org) - A Free and Open Source Java Framework for Multiobjective Optimization
  - [DGantt](http://sourceforge.net/projects/dgantt/) - A simple yet powerful Gantt chart library for Java 1.6 and later
  - [SVN Backups](https://github.com/dhadka/SVN-Backups) - A Python script for creating full or incremental SVN dumps and uploading the result to Dropbox
