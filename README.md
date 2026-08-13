# Dallas County Residential Pipeline Map

De-identified, aggregated WGS84 GeoJSON for the Dallas County GIS data
challenge. It contains subdivision-level project attributes only and excludes
owner, taxpayer, and mailing-address fields.

The geometry is a 10-foot topology-preserving simplification for browser
display. Project counts and business attributes are unchanged from the audited
output; the presentation files add only display styles and rank markers.

Recommended views:

- [presentation_map](https://geojson.io/#data=data:text/x-url,https%3A%2F%2Fraw.githubusercontent.com%2FBadLee2018%2Fdallas-county-residential-pipeline-map%2Fmain%2Fdallas_active_residential_presentation.geojson) - 401 Active Residential projects, with Top 5 highlighted.
- [top5_map](https://geojson.io/#data=data:text/x-url,https%3A%2F%2Fraw.githubusercontent.com%2FBadLee2018%2Fdallas-county-residential-pipeline-map%2Fmain%2Fdallas_top5_residential_projects.geojson) - five boundaries plus ranked centroid markers.
- [full_audit_map](https://geojson.io/#data=data:text/x-url,https%3A%2F%2Fraw.githubusercontent.com%2FBadLee2018%2Fdallas-county-residential-pipeline-map%2Fmain%2Fdallas_residential_pipeline_display.geojson) - all 1,477 high-confidence projects.

Scope: high-confidence spatial subset only; not a claim of complete countywide
coverage. `active_residential` is based on recent official structure evidence,
not a building-permit assertion. Source-null subdivision numbers and cities are
left null rather than inferred.
