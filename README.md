# This is a collection of templates for Perspect.

The directory stucture of the templates is important.  There is a top-level directory called "templates" and within that is each template.  Within each individual template directory are Jinja templates and a "static" directory containing static assets.  

On the back-end, Perspect stores static assets separately from Jinja templates.  Static assets are publicly accessible and stored in "<template_name>/static/..."  

Here is an example with the attilla template:

```<link href="/attilla/static/css/style.css" type="text/css" rel="stylesheet" />```

There are two objects accessible within the templates: posts and site.  The following is a description of each.

***posts*** (list) -- All posts associated with a site_name
+  post (dict)    
    + link (string)
    + post_author (string)
    + post_content (string)
    + post_date_gmt (gmt_date)
    + post_id (int)
    + post_modified_gmt (gmt_date)
    + post_status (string)
    + post_title (string)
    + post_type (string)
    + site_name (string)
    + slug (string)
    


***site*** (dict)  -- Information about the site
+ administrators (list)
+ authors (list)
+ contributors (list)
+ domain (string)
+ editors (list)
+ owner (string)
+ protocol (string)
+ site_name (string)


# Refer to import of macro/pagination.html in the hyde template's index.html file to use pagination
