# OpenTails

A Python-first Linux distribution with its own desktop environment, tools, and ecosystem.

«OpenTails is still heavily in development. Expect things to break. A lot.»

# What is OpenTails?

OpenTails is a Linux distribution built around a simple idea:

Use Linux for the low-level stuff, and Python for as much of the operating system experience as possible.

Linux handles the parts that require serious low-level hardware support, such as:

- Hardware drivers
- Memory management
- Process management
- Filesystems
- Networking
- Graphics
- Hardware compatibility

OpenTails builds on top of that with its own:

- Python-based system software
- Shell
- Desktop environment
- Applications
- Package-management experience
- Configuration tools
- User experience

The goal isn't to reinvent the Linux kernel.

The goal is to build an operating system experience on top of Linux, while keeping Python at the heart of OpenTails.

# Dekx

Dekx is the desktop environment for OpenTails.

It is intended to provide the graphical experience of the operating system, including:

- Windows
- Panels
- Menus
- Application launching
- Desktop management
- System tools
- OpenTails-specific UI

The default visual style is planned to be pixel-art inspired.

# Packages

OpenTails uses ".deb" packages as its primary package format.

This means OpenTails can build on the huge ecosystem that already exists around Debian packages instead of inventing an entirely new package format.

The planned package-management interface is:

ot install <package>
ot remove <package>
ot update
ot upgrade
ot search <package>

The long-term goal is for installing software to feel like a native OpenTails experience while still benefiting from the existing Linux software ecosystem.

# Architecture

The planned architecture looks roughly like this:

                 OpenTails
                     │
        ┌────────────┴────────────┐
        │                         │
      Dekx                  OpenTails Shell
        │                         │
        └────────────┬────────────┘
                     │
             OpenTails Services
                     │
                Python Runtime
                     │
              Linux Userspace
                     │
                Linux Kernel
                     │
                  Hardware

This isn't the final architecture yet. OpenTails is still being developed, so parts of this design may change.

# Why Python?

Python is the main language behind the OpenTails project because it makes it possible to develop system software and applications quickly without having to write everything in a low-level language.

Python is especially useful for:

- System utilities
- Shell components
- Desktop applications
- Configuration tools
- Package-management tools
- Prototyping
- OpenTails applications

Low-level components that Python cannot reasonably handle will be provided by Linux and other lower-level components.

# Applications

OpenTails applications are intended to integrate with Dekx and the OpenTails system.

The long-term goal is to make creating an OpenTails application as approachable as possible, especially for Python developers.

A future OpenTails application might look something like:

my-app/
├── app.py
├── manifest
├── icon.png
└── assets/

and eventually be distributed as a ".deb" package.

# Current Status

OpenTails is early in development.

Currently, the project is primarily focused on building the foundations of the system.

Expect:

- Missing features
- Experimental code
- Broken things
- Major architecture changes
- Probably some questionable decisions

That's part of the process.

# Roadmap

The roadmap is not set in stone, but the general direction is:

- [x] Start the OpenTails project
- [x] Establish the Python-first concept
- [x] Plan Dekx
- [x] Choose Linux as the kernel foundation
- [x] Choose ".deb" as the primary package format
- [ ] Build the OpenTails shell
- [ ] Build core OpenTails services
- [ ] Begin Dekx development
- [ ] Create the OpenTails application API
- [ ] Build the OpenTails package manager
- [ ] Build native OpenTails applications
- [ ] Create a bootable OpenTails image
- [ ] Test OpenTails in QEMU
- [ ] Test on real hardware
- [ ] Create installable OpenTails releases

# Development

OpenTails is primarily written in Python.

The project is developed with experimentation in mind. The architecture may change significantly as development progresses.

For safe early testing, virtualization such as QEMU can be used before attempting to boot OpenTails on physical hardware.

# License

OpenTails is licensed under the GNU General Public License v3.0.

See ""LICENSE"" (LICENSE) for the full license.

Branding

OpenTails and Dekx are project names and branding.

The software is open source under GPL-3.0, while the project's branding may be subject to separate rules.

---

OpenTails — Linux underneath. Python at the heart.
