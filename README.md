# Shibboleth-IdP-Throttling-patch

## This patch adds throttling for both usernames and IP addresses ##

## Install ##

# Download the source code
svn co https://svn.shibboleth.net/java-identity-provider/tags/3.2.1/ 3.2.1

# Patch it
patch -p0 -i ../p.patch

# Build
cd 3.2.1/idp-parent && mvn -DskipTests clean install

## Why skip tests? ##
Because the current tests breaks the patch

## Problems or questions ##
Send me an email: victor.naslund@smhi.se
