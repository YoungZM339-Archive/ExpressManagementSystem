# ExpressManagementSystem

A C++17 command-line parcel-management course project. The program loads user and parcel data from local configuration files, provides post-login flows for shipping, receiving, balances, and parcel status, and writes updated data back on exit.

## Feature Scope

- User login and user-information management.
- User balance data.
- Sender, recipient, and parcel information.
- Delivery status and courier information.
- Persistence through local configuration-file reads and writes.

## Build

Requires CMake 3.24 or later and a C++17-compatible compiler.

    cmake -S . -B build
    cmake --build build

Run the generated `ExpressManagementSystem` executable from the repository root or from a working directory that preserves the same data-directory structure.

## Data Files

- `UsersDir/Users.config`: User data.
- `ItemsDir/Items.config`: Parcel data.

The program reads these files at startup and writes updated results on exit. Back up your own test data before running it, and do not commit real personal information or real logistics records to version control.

## Intended Use

This project is for practicing C++ class design, file I/O, and command-line flow organization. It does not include the identity security, concurrency handling, network communication, reliable tracking, privacy compliance, or disaster recovery expected of a production logistics system.

## License

The repository currently has no declared license.