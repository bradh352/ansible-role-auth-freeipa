# Authentication Enrollment for FreeIPA Role

Author: Brad House<br/>
License: MIT<br/>
Original Repository: https://github.com/bradh352/ansible-role-auth-freeipa

## Overview

FreeIPA is an open source identity and authorization provider that combines
Kerberos and LDAP to secure enterprise systems.

This role is used to join a host to a pre-existing FreeIPA domain.

## Variables used by this role

In most environments these settings will likely be global and stored under the
group `all` vars.

* `auth_freeipa_enroll_user`: Username to use to enroll the system into the
  FreeIPA realm.
* `auth_freeipa_enroll_pass`: Password for the enrollment user in order to
  enroll the host.  Should be stored in the ansible vault.
* `auth_freeipa_server`: The freeipa server to use for enrollment.

