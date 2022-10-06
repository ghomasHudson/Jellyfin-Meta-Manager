# Cannes Default Metadata File

The `- pmm: cannes` Metadata File is used to  create collections based on the Cannes Film Awards.

This Default file requires [Trakt Authentication](https://metamanager.wiki/en/latest/config/trakt.html)

Example Collections Created:

![](../images/cannes.png)

The below YAML in your config.yml will create the collections:
```yaml
libraries:
  Movies:
    metadata_path:
      - pmm: cannes
```



## Template Variables

Template Variables can be used to manipulate the file from the default settings which are provided. 

Note that the `templates_variables:` section only needs to be used if you do want to actually change how the defaults work. Any value not specified is just ignored.

All [Shared Variables](../variables) are available as well as the additional Variables below which can be used to customize the file.

| Variable               | Description & Values                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|:-----------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `use_year_collections` | **Description:** Turn the individual year collections off<br>**Values:** `false` to turn of the collections                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| `collection_order`     | **Description:** Changes the Collection Order<br>**Values:**<table class="clearTable"><tr><td>`release`</td><td>Order Collection by Release Dates</td></tr><tr><td>`alpha`</td><td>Order Collection Alphabetically</td></tr><tr><td>`custom`</td><td>Order Collection Via the Builder Order</td></tr><tr><td>[Any `plex_search` Sort Option](../builders/plex.md#sort-options)</td><td>Order Collection by any `plex_search` Sort Option</td></tr></table>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| `data`                 | **Description:** Changes the values of the collections<br>**Values:**<br><table class="clearTable"><tr><th>Attribute</th><th>Description & Values</th></tr><tr><td><code>starting</code></td><td>Controls the starting year for collections</br><strong>Values:</strong> Number greater than 0</td><td><strong>Default:</strong> current_year-5</td></tr><tr><td><code>ending</code></td><td>Controls the ending year for collections</br><strong>Values:</strong> Number greater than 1</td><td><strong>Default:</strong> current_year</td></tr><tr><td><code>increment</code></td><td>Controls the incriment (i.e. every 5th year)</br><strong>Values:</strong> Number greater than 0</td><td><strong>Default:</strong> 1</td></tr></table><ul><li><strong><code>starting</code> and <code>ending</code> can also have the value <code>current_year</code></strong></li><li><strong>You can also use a value relative to the <code>current_year</code> by doing <code>current_year-5</code></strong></li></ul> |

The below shows an example config.yml with all the template_variables set away from their defaults:

```yaml
libraries:
  Movies:
    metadata_path:
      - pmm: cannes
        template_variables:
          collection_section: 8
          collection_mode: show_items
          collection_order: alpha
          radarr_add_missing: true
```