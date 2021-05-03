FROM ten7/flightdeck-web-7.4
MAINTAINER tess@ten7.com

# This has to be re-run on each variant image, apparently.
USER root
RUN setcap cap_net_bind_service=+ep /usr/sbin/httpd

# Use drush to 8.x for Drupal 7
USER apache
ENV DRUSH_VERSION "8.x"
