# Django Settings

## Managing Django Settings: Issues

    Different environments. Usually, you have several environments: local, dev, ci, qa, staging, production, etc. You need an approach that allows you to keep all these Django setting configurations.

    Sensitive data. You have SECRET_KEY in each Django project. On top of this there can be DB passwords and tokens for third-party APIs like Amazon or Twitter. This data cannot be stored in VCS.

    Sharing settings between team members. You need a general approach to eliminate human error when working with the settings.

## Setting Configuration: Different Approaches

    settings_local.py This is the oldest method. I used it when I was configuring a Django project on a production server for the first time. I saw a lot of people use it back in the day, and I still see it now.

    Separate settings file for each environment - This is an extension of the previous approach. It allows you to keep all configurations in VCS and to share default settings between developers.

## 12 Factors

    Codebase
    Dependencies
    Config
    Backing services
    Build, release, run
    Processes
    Port binding
    Concurrency
    Disposability
    Dev/prod parity
    Logs
    Admin processes

## Django Settings: Best practices

    Keep settings in environment variables.
    Write default values for production configuration (excluding secret keys and tokens).
    Don’t hardcode sensitive settings, and don’t put them in VCS.
    Split settings into groups: Django, third-party, project.
    Follow naming conventions for custom (project) settings.

## What is SSH

    SSH, or Secure Shell, is a remote administration protocol that allows users to control and modify their remote servers over the Internet.

    It provides a mechanism for authenticating a remote user, transferring inputs from the client to the host, and relaying the output back to the client.

## Symmetric Encryption

    Symmetric encryption is a form of encryption where a secret key is used for both encryption and decryption of a message by both the client and the host.

    Symmetrical encryption is often called shared key or shared secret encryption. There is usually only one key that is used, or sometimes a pair keys where one key can easily be calculated using the other key.

## Asymmetric Encryption

    Unlike symmetrical encryption, asymmetrical encryption uses two separate keys for encryption and decryption. These two keys are known as the public key and the private key. Together, both these keys form a public-private key pair.

## Hashing

    One-way hashing is another form of cryptography used in Secure Shell Connections. One-way-hash functions differ from the above two forms of encryption in the sense that they are never meant to be decrypted.
