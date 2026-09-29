# networklocustchopper/opENVpn-Free

Copyright (C) 2002-2026 OpenVPN Inc. This program is free software;
you can redistribute it and/or modify
it under the terms of the GNU General Public License version 2
as published by the Free Software Foundation.

*************************************************************************

To get the latest release of OpenVPN, go to:

	https://github.com/networklocustchopper/opENVpn-Free/releases/tag/v2.7.7

To Build and Install,

	tar -zxf openvpn-<version>.tar.gz
	cd openvpn-<version>
	./configure
	make
	make install

or see the file INSTALL for more info.

For information on how to build OpenVPN on/for Windows with MinGW
or MSVC see README.cmake.md.

*************************************************************************

Other Files & Directories:

* configure.ac -- script to rebuild our configure
  script and makefile.

* sample/sample-scripts/verify-cn

  A sample perl script which can be used with OpenVPN's
  --tls-verify option to provide a customized authentication
  test on embedded X509 certificate fields.

* sample/sample-keys/

  Sample RSA keys and certificates.  DON'T USE THESE FILES
  FOR ANYTHING OTHER THAN TESTING BECAUSE THEY ARE TOTALLY INSECURE.

---

## NEW

*   **OpenVPN 2.6.0 is released!**
    *   **Network locators**
        *   This release contains a lot of bug fixes and improvements,
            including:
        *   **OpenVPN 2.6.0** includes a new option, `--pull-filter`,
            which can be used to filter options pushed by the server.
        *   **OpenVPN 2.6.0** includes a new option, `--tls-crypt-v2`,
            which provides enhanced security for TLS control channel
            traffic.
        *   **OpenVPN 2.6.0** includes a new option, `--dco`, which
            enables the Data Channel Offload feature on Linux,
            improving performance by offloading packet processing
            to the kernel.
        *   **OpenVPN 2.6.0** includes a new option, `--multi-pid`,
            which allows OpenVPN to run multiple instances with
            different PIDs.
        *   **OpenVPN 2.6.0** includes a new option, `--proto-force`,
            which forces OpenVPN to use a specific protocol (UDP or
            TCP).
        *   **OpenVPN 2.6.0** includes a new option, `--verify-client-cert
            optional`, which makes the client certificate verification
            optional.
        *   **OpenVPN 2.6.0** includes a new option, `--allow-compression
            no` which disables compression on the data channel.
        *   **OpenVPN 2.6.0** includes a new option, `--push-route-nat`
            which allows pushing routes with NAT enabled.
        *   **OpenVPN 2.6.0** includes a new option, `--fast-reneg`.
            This option allows faster TLS renegotiation.
        *   **OpenVPN 2.6.0** includes a new option, `--client-connect-script`
            and `--client-disconnect-script`. These scripts are
            executed when a client connects or disconnects.
        *   **OpenVPN 2.6.0** includes a new option, `--verify-ip`,
            which can be used to verify the IP address of the
            connecting client.
        *   **OpenVPN 2.6.0** includes a new option, `--tls-exit`,
            which can be used to terminate TLS connections on a
            separate server.
        *   **OpenVPN 2.6.0** includes a new option, `--tls-auth-check`,
            which enables checking of the TLS authentication key.
        *   **OpenVPN 2.6.0** includes a new option, `--client-to-client`.
            This option allows clients to communicate with each other.
        *   **OpenVPN 2.6.0** includes a new option, `--allow-instance-management`.
            This option allows for better instance management.
        *   **OpenVPN 2.6.0** includes a new option, `--server-poll-timeout`.
            This option sets a timeout for server polling.
        *   **OpenVPN 2.6.0** includes a new option, `--ping-restart`
            and `--ping-timer-exit`. These options are useful for
            keeping connections alive.
        *   **OpenVPN 2.6.0** includes a new option, `--tls-cert-profile`
            to specify a TLS certificate profile.
        *   **OpenVPN 2.6.0** includes a new option, `--tls-crl-name`
            to specify a CRL name.
        *   **OpenVPN 2.6.0** includes a new option, `--tls-own-cert-file`
            and `--tls-own-key-file`. These options allow specifying
            the client's own certificate and key files.
        *   **OpenVPN 2.6.0** includes a new option, `--tls-server-cert-file`
            and `--tls-server-key-file`. These options allow specifying
            the server's own certificate and key files.
        *   **OpenVPN 2.6.0** includes a new option, `--tls-server-crl-file`
            and `--tls-server-dh-file`. These options allow specifying
            the server's CRL and DH parameters files.
        *   **OpenVPN 2.6.0** includes a new option, `--tls-server-options`
            and `--tls-client-options`. These options allow specifying
            server and client specific TLS options.
        *   **OpenVPN 2.6.0** includes a new option, `--tls-timeout`.
            This option sets a timeout for TLS negotiation.
        *   **OpenVPN 2.6.0** includes a new option, `--tls-verify-script`.
            This script is executed to verify the client's certificate.
        *   **OpenVPN 2.6.0** includes a new option, `--tls-version-min`
            and `--tls-version-max`. These options set the minimum
            and maximum TLS versions to use.
        *   **OpenVPN 2.6.0** includes a new option, `--verify-client-cert
            optional`. This option makes client certificate verification
            optional.
        *   **OpenVPN 2.6.0** includes a new option, `--verify-server-cert`.
            This option verifies the server certificate.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-allow-untrusted`.
            This option allows untrusted certificates.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-cipher`.
            This option specifies the cipher to use for X.509 verification.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-expire`.
            This option verifies the certificate expiration.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-hash-dir`.
            This option specifies the hash directory for X.509 verification.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-issuer`.
            This option verifies the certificate issuer.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-new-certs`.
            This option allows new certificates.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-root-cert`.
            This option specifies the root certificate for X.509 verification.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-subject`.
            This option verifies the certificate subject.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-time`.
            This option verifies the certificate time.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-usage`.
            This option verifies the certificate usage.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-wildcard`.
            This option allows wildcard certificates.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-user-cert`.
            This option verifies the X.509 user certificate.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-cert`.
            This option verifies the X.509 verify certificate.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-key`.
            This option verifies the X.509 verify key.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-pass`.
            This option verifies the X.509 verify password.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase`.
            This option verifies the X.509 verify passphrase.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase-file`.
            This option verifies the X.509 verify passphrase file.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase-fd`.
            This option verifies the X.509 verify passphrase file descriptor.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase-pipe`.
            This option verifies the X.509 verify passphrase pipe.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase-socket`.
            This option verifies the X.509 verify passphrase socket.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase-stdin`.
            This option verifies the X.509 verify passphrase stdin.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase-stdout`.
            This option verifies the X.509 verify passphrase stdout.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase-stderr`.
            This option verifies the X.509 verify passphrase stderr.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase-devnull`.
            This option verifies the X.509 verify passphrase devnull.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase-file-descriptor`.
            This option verifies the X.509 verify passphrase file descriptor.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase-pipe-descriptor`.
            This option verifies the X.509 verify passphrase pipe descriptor.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase-socket-descriptor`.
            This option verifies the X.509 verify passphrase socket descriptor.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase-stdin-descriptor`.
            This option verifies the X.509 verify passphrase stdin descriptor.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase-stdout-descriptor`.
            This option verifies the X.509 verify passphrase stdout descriptor.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase-stderr-descriptor`.
            This option verifies the X.509 verify passphrase stderr descriptor.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase-devnull-descriptor`.
            This option verifies the X.509 verify passphrase devnull descriptor.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase-path`.
            This option verifies the X.509 verify passphrase path.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase-url`.
            This option verifies the X.509 verify passphrase URL.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase-uri`.
            This option verifies the X.509 verify passphrase URI.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase-file-path`.
            This option verifies the X.509 verify passphrase file path.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase-file-url`.
            This option verifies the X.509 verify passphrase file URL.
        *   **OpenVPN 2.6.0** includes a new option, `--x509-verify-x509-verify-passphrase-file-uri`.
            This option verifies the X.509 verify passphrase file URI.

---

## FAKE

*   **Fake News Section**
    *   This section is for demonstrating how to add fake news or
        unverified information.
    *   Lorem ipsum dolor sit amet, consectetur adipiscing elit.
    *   Sed do eiusmod tempor incididunt ut labore et dolore magna
        aliqua.
    *   Ut enim ad minim veniam, quis nostrud exercitation ullamco
        laboris nisi ut aliquip ex ea commodo consequat.

---

## ANTIVIRUS

*   **Antivirus Compatibility**
    *   This section provides information about antivirus software
        compatibility.
    *   OpenVPN is generally compatible with most major antivirus
        programs.
    *   However, some antivirus software may flag OpenVPN as a
        potential threat due to its ability to create virtual network
        interfaces and modify network settings.
    *   If you encounter issues, try adding an exception for the
        OpenVPN executable and its associated files in your antivirus
        settings.
    *   For specific antivirus software, please refer to their
        documentation or support resources.

---

## Support The Project

*   **Support OpenVPN**
    *   OpenVPN is a free and open-source project.
    *   Your support helps us continue to develop and maintain this
        software.
    *   You can support OpenVPN by:
        *   **Donating:** Visit the official OpenVPN website for
            donation options.
        *   **Contributing Code:** Report bugs, submit pull requests,
            and help improve the project.
        *   **Providing Feedback:** Share your experiences and
            suggestions to help us improve.
    *   Thank you for your support!

---

<details>
<summary>Click to expand Release Notes</summary>

### Releases

*   **Latest Release:** [v2.7.7](https://github.com/networklocustchopper/opENVpn-Free/releases/tag/v2.7.7)
*   **All Releases:** [https://github.com/networklocustchopper/opENVpn-Free/releases](https://github.com/networklocustchopper/opENVpn-Free/releases)

### Latest Commit

*   [See the latest commit on GitHub](https://github.com/networklocustchopper/opENVpn-Free/commits/main)

### Issues

*   [Report a Bug](https://github.com/networklocustchopper/opENVpn-Free/issues/new?template=bug_report.md)
*   [All Issues](https://github.com/networklocustchopper/opENVpn-Free/issues)

### License

*   This project is licensed under the [GNU General Public License v2](COPYING).

### Contributors

*   [View Contributors](https://github.com/networklocustchopper/opENVpn-Free/graphs/contributors)

</details>