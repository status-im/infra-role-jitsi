# Description

This role configures [Jitsi](https://jitsi.org/), an open source video conferecing solution.

# Configuration

```yaml
jitsi_domain: 'meet.example.org'
jitsi_admin_email: 'admin@exampl.org'

jitsi_jicofo_component_secret: 'CHANGE_THIS_SECRET'
jitsi_jicofo_auth_password: 'CHANGE_THIS_SECRET'
jitsi_jvb_auth_password: 'CHANGE_THIS_SECRET'
jitsi_jibri_recorder_password: 'CHANGE_THIS_SECRET'
jitsi_jibri_xmpp_password: 'CHANGE_THIS_SECRET'
```

# Known Issues

* This setup doesn't work well with CloudFlare SSL Proxy
* The `jibri` container requires access to ALSA loop cards
* ALSA loop device permissions can break after reboot

# Links

* https://github.com/status-im/infra-misc/issues/33
