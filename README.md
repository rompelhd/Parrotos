# Parrotos

Parrot OS RootFS
This repository provides a Parrot OS RootFS, which can be used in both chroot and proot environments. Parrot OS is a security-focused, Debian-based distribution commonly used for penetration testing, digital forensics, and development.

RootFS for chroot/proot
What is a RootFS?
A Root Filesystem (RootFS) refers to the complete directory structure and files necessary to provide a fully functional operating system environment. It typically includes directories like /bin, /etc, /home, /usr, and others, which hold the essential binaries, libraries, configuration files, and user files that make up the operating system.

When using a RootFS in environments like chroot or proot, you essentially encapsulate an entire operating system into a self-contained directory that can be used independently of the host operating system.

What is chroot?
chroot (change root) is a Unix command that changes the root directory for the current running process and its children. This essentially gives the illusion of running a different operating system environment by isolating processes within a specific directory structure (the RootFS). However, chroot requires root privileges to operate and doesn't handle certain system resources like mounting filesystems or devices.