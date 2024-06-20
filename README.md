## INTRODUCTION

The BD Embargo module is a set of configurations and migrations to facilitate time-based embargoing of content.

The main components are:

- A 'Embargo' tag for the Islandora Access vocabulary
- A group type and associated configurations.
- A context to trigger the 'Metadata-only' view from BD Core
- A field for embargo date
- A view to show all items tagged with Embargo whose embargo dates are older than the current date and time.
    - This view contains a Views Bulk Edit field that can be called from a Cron command to unset the Embargo tag.

The ## INSTALLATION

Install as you would normally install a contributed Drupal module.
See: https://www.drupal.org/node/895232 for further information.

Then import the Embargo access tag:

```shell
drush migrate:import bd_embargo_tags
```

## MAINTAINERS

- Alexander O'Neill - alexander@born-digital.com
- Danny Lamb - daniel@born-digital.com
