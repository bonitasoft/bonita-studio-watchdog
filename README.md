# bonita-studio-watchdog

**Archived Repository**: the watchdog is now directly integrated within the Bonita Studio as of Bonita 7.10

This project aims to ensure that the Studio Tomcat instance is always shutdown even after a Studio crash.

A dedicated webapp (deployed within the Tomcat instance bundled within the Studio) regularly performs a healthcheck on the Studio; if it is not reachable, the webapp ask for a Tomcat shutdown.
