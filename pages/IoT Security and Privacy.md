- VL 5b Beispiele anschauen
- Securing IoT
	- Security
		- General best practices
			- Avoid common issues:
				- Buffer overflows
				- SQL injections
				- etc..
			- Input validation
			- Secure defaults
			- Overall system design
		- May also need to consider hardware security
		  — Tamper-proof devices
			- However: Often IoT devices are not designed with security in mind from the start.
- Cryptography
	- consider low-power devices
		- Common protocols (SSL/TLS) often too heavy
		- RSA too heavy for very low-powered devices
		- ECC can be acceptable, but still slow
	- Main things to consider:
		- Confidentiality
		- Integrity
		- Authentication
	- Main focus on symmetric cryptography:
		- AES128 can perform well even on 8bit micro-controllers
		- Block cipher based MACs
		- SipHash (but is short)
		- SHA family comparatively slow
		- Issue!
			- Shared Keys
- Privacy
	- Requirements
		- Secure implementations
		- Additional care take to:
			- Minimize personal data being stored/processed
			- Where possible, process locally
			- Where necessary, store encrypted
			- Trust considerations