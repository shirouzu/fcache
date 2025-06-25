# Clear file cache for Windows(x64)
This tool deletes all file cache for accurate copy benchmarks.  
(it requires admin privileges.)

This tool just issues only two system calls.
```
 NtSetSystemInformation(SystemMemoryListInformation, &MemoryFlushModifiedList,...)
 NtSetSystemInformation(SystemMemoryListInformation, &MemoryPurgeStandbyList,...)
```
