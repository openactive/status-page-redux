# status-page-redux

Updated OpenActive status page, auto-generated from DCAT data catalogue

## Background

For reference, the existing status page can be found at [https://status.openactive.io/](https://status.openactive.io/). The code for the page is available at the relevant [GitHub repo](https://github.com/openactive/api-dashboard).

A previous attempt at building a (much more ambitious) replacement status page can be found in the [conformance-status-page](https://github.com/openactive/conformance-status-page) repository. This status page was to have conducted much more thorough validation and standards conformance-checking (and to have reported statistics regarding this to the end-user). However, data variability meant that reporting and analysis proved onerous and, ultimately, untenable.

## Intended Functionality

The purpose of redux status page is simply to provide an updated version of the current status page, with the following changes:

1. The list of websites will be auto-generated from a [DCAT data catalogue](https://openactive.io/data-catalogs/data-catalog-collection.jsonld), spidering down through the provided links until reaching nodes representing individual dataset sites.
1. The columns 'Uses Paging Spec', 'Uses Opportunity Model', 'Includes coordinates', and 'Summary' will be removed.
2. Columns for 'Facilities', 'Events', and 'Sessions' will be added. Values will be boolean.
3. The list will be sortable alphabetically
1. The display will be paginated
1. A link will be provided to the originating DCAT data catalogue
1. The UI and UX will not be so rubbish
