# Healthcheck containers showing unhealthy

- Shell scripts copied from Windows to Linux lost their executable bit, so the container health checks failed.
- Fix: chmod +x on the scripts, and a .gitattributes file with "*.sh text eol=lf" so line endings stay Linux-style.
- Lesson: docker inspect shows the health check log, which tells you why a container is unhealthy.
