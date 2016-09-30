# Open Data Schema Mapping in DKAN

Placeholder for ODSM DKAN module when moves into core.

-------

With DKAN it is easy to [Add New Fields](/dkan-documentation/dkan-developers/adding-fields-dkan) which become part of the form and page view. To add the new field to the output of one of DKAN's APIs such as "package_show" or "data.json", install the [Open Data Schema Mapper](https://github.com/NuCivic/open_data_schema_map) and [Open Data Schema Mapper DKAN](https://github.com/NuCivic/open_data_schema_map_dkan) modules if they are not already included in your version of DKAN. See Open Data Schema Mapper's [README](https://github.com/NuCivic/open_data_schema_map/blob/master/README.md) for more details about that module.

## Adding "MY NEW FIELD" to package_show Endpoint

To add the output from MY NEW FIELD to the package_show endpoint 

+ Go to ```/admin/config/services/odsm/edit/ckan_resource_show```
+ Choose a field to add the output to:

![open data schema mapper](http://docs.getdkan.com/sites/default/files/Screen%20Shot%202014-10-02%20at%202.43.49%20PM.png)

+ Click or select the token for "MY NEW FIELD" under "Replacement Patterns"

![token list](http://docs.getdkan.com/sites/default/files/Screen%20Shot%202014-10-02%20at%202.45.33%20PM.png)

+ Make sure token is placed in desired field:

![value entered](http://docs.getdkan.com/sites/default/files/Screen%20Shot%202014-10-02%20at%202.45.51%20PM.png)

+ Click **Save**
+ Output from "MY NEW FIELD" should be visible in package_show endpoint:

![endpoint](http://docs.getdkan.com/sites/default/files/package_show_Example.png)

Note that the "position" field now has the value from a node we created with "MY NEW FIELD" in the <a href="/dkan-documentation/dkan-developers/adding-fields-dkan">Add New Fields</a> example.