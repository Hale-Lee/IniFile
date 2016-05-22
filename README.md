# IniFile

It's a very simple way to access *.ini File, the source code is written by C++/MFC 

usage:
  
  // structor/constructor
  CIniFile(LPCTSTR szFileName);
	virtual ~CIniFile();
	
	
  // Open Close file.
	BOOL Open(BOOL isReadOnly = FALSE);
	
	BOOL Close();

  // read/write method
	int GetKeyVal(CString szSectionName, CString szKeyName, int ipDefault);
	
	CString GetKeyVal(CString szSectionName, CString szKeyName, LPCTSTR szDefault);
	
 	BOOL WriteValue(LPCTSTR szSection, LPCTSTR szItem, LPCTSTR szValue, LPCTSTR szComment = NULL);
	
