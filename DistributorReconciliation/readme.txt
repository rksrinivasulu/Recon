1) Unzip the reconcilation_config_files_3.0.0.0 file
2) Change the below files
	i) reconcilation.sh
	ii) Reconcilation\properties\PoolBundle.properties
	iii) Log4j.properties

reconcilation.sh
----------------

JAVA_HOME="Java Path"

PoolBundle.properties
----------------------
DB Details:
----------
recon.db.url=DB URL Which is available in Oracle DS(jdbc:oracle:thin:@192.168.149.114:1521:LOOPENTDB)
recon.db.username=DB User Name(MEX_GEO)
recon.db.password=DB User Password(MEX_GEO)


RECONCILATION_FILES_LOCAL_PATH --> Local file path for Reconcilation FTP files (D:/jboss-5.1.0.GA/server/paymgr/docs/ReconcilationFiles)
RECONCILATION_PROCESSED_FILES_LOCAL_PATH ----> Local file path for Reconcilation processed file path(D:/jboss-5.1.0.GA/server/paymgr/docs/ReconcilationProcessedFiles)

FTP Details:
-----------

PROCESSED_FILEUPLOAD_DIRECTORY=Reconcilation processed file path in FTP(/mtt/ReconcilationFilesProcessed)
ftpserver.ipaddress=FTP IP address(10.194.50.20)
ftpserver.username=FTP User Name(mtt)
ftpserver.password=FTP Password(xius123)
ftp.server.folder=FTP Reconcilation source file location(ReconcilationFiles)

log4j.properties.path=Log4j Properties location(D:/Reconcilation/properties/Log4j.properties)

Log4j.properties:
----------------
log4j.appender.R.File=(Log file place location)D:/Reconcilation/dist/Reconcilation/log/reconcilation.log

3) to start the Reconcilation application use "Start_reconcilation.sh" file
4) to stop the Reconcilation application use "Stop_reconcilation.sh" file
  




