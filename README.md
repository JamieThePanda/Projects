# Projects
Projects / Real World Applications
🛠️ Windows Login Issue & System Recovery – Incident Summary
Issue:
Unexpectedly locked out of my Windows laptop after years of using the same password. System displayed a "failed sign-in attempts" message and requested a 2-hour wait before retrying. Even after waiting overnight, the issue persisted.

Steps Taken:

Initial Diagnostics:

Attempted Safe Mode login – unsuccessful.

Reviewed Netstat for unusual connections – nothing suspicious found.

Ran full antivirus scan — came back clean.

Password Reset:

Successfully reset my Microsoft password using account recovery tools.

Gained temporary access, but issue repeated on reboot.

Command Line Recovery:

Entered Windows Recovery Environment (WinRE).

Accessed X:\Windows\System32 via Command Prompt.

Ran sfc /scannow — initially failed in Safe Mode.

Successfully ran sfc /scannow from full OS login — detected and repaired corrupted system files.

Ran DISM /Online /Cleanup-Image /RestoreHealth — partial success, Error: 2 reported but no critical errors remained.

Resolution:

Regained full access to the system.

Verified system health and security status.

Implemented a long, complex password and enabled additional security measures.

🔐 Key Takeaways
Critical thinking & persistence: Navigated a multi-step issue calmly and methodically.

System integrity skills: Learned to use sfc, DISM, and Command Prompt for diagnostics and repair.

Security mindset: Took immediate action to secure account and verify system integrity.
