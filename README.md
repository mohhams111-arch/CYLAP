# CYLAP
# Super SSH

## Objective
Connect to a remote server using SSH and retrieve the flag.

## Solution

```bash
ssh ctf-player@titan.picoctf.net -p <PORT>
```

- Accepted the SSH fingerprint by typing `yes`.
- Entered the provided password.
- Successfully connected and obtained the flag.

## Issues Encountered

- **Connection refused:** Used an old port after the instance restarted.
- **Permission denied:** Entered the password incorrectly.

## What I Learned

- How to use the `ssh` command.
- Purpose of `Host`, `Username`, and `Port`.
- Difference between **Connection Refused** and **Permission Denied**.


# What's a Net Cat?

## Objective
Connect to a remote server using Netcat (`nc`) and retrieve the flag.

## Solution

```bash
nc fickle-tempest.picoctf.net <PORT>
```

The server immediately returned the flag after the connection was established.

## Issues Encountered

- **Connection refused:** The instance had restarted, so the port changed.
- **Solution:** Restarted the instance and used the new port.

## What I Learned

- Basic usage of the `nc` command.
- How to connect to a remote TCP service.
- Difference between SSH and Netcat.
