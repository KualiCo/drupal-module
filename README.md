# kualico-cm-drupal-module
This drupal module is meant to simplify the interaction with the CM api in Drupal.

Alone it will display nothing other than its own config page, where the user will enter the details specific to their
CM instance. When enabled and configured, you can use the methods provided in your development of drupal modules that
need data from the CM API (e.g. course catalogs, program details, etc).

This module exposes five externally useful functions. Four of them are the basic types of requests that the CM API accepts namely:
cm_drupal_get($url)
cm_drupal_post($url [,$body = null])
cm_drupal_put($url [,$body = null])
cm_drupal_delete($url [,$body = null])

The fifth is a basic ajax method where the request type is specified in the parameters:
cm_drupal_ajax($url [, $method = 'GET', $body = null])

Each function returns the JSON response from the
server.

# Installation

Copy cm_drupal.info and cm_drupal.module to $yourdrupalpath/sites/all/modules/cm_drupal

Clear your caches and enable the module in the Drupal administration>modules page.

mikec@kuali.co
