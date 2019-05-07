# ![LOGO](logo.png) Botify **flow**ground Connector

## Description

A generated **flow**ground connector for the Botify API (version 1.0.0).

Generated from: https://api.apis.guru/v2/specs/botify.com/1.0.0/swagger.json<br/>
Generated at: 2019-05-07T17:39:46+03:00

## API Description

Botify Saas API

## Authorization

Supported authorization schemes:
- API Key
## Actions

### List all analyses for a project

*Tags:* `Project`

#### Input Parameters
* `page` - _optional_ - Page Number
* `size` - _optional_ - Page Size
* `only_success` - _optional_ - Return only successfully finished analyses
* `fields` - _optional_ - Which fields to return (comma-separated)

### Get an Analysis detail

*Tags:* `Analysis`

#### Input Parameters
* `previous_crawl` - _optional_ - Previous analysis identifier
* `project_slug` - _required_ - Project's identifier
* `analysis_slug` - _required_ - Analysis' identifier

### Update an Analysis' attribute

*Tags:* `Analysis`

#### Input Parameters
* `username` - _required_ - User's identifier
* `project_slug` - _required_ - Project's identifier
* `analysis_slug` - _required_ - Analysis' identifier

### Return global statistics for an analysis

*Tags:* `Analysis`

#### Input Parameters
* `username` - _required_ - User's identifier
* `project_slug` - _required_ - Project's identifier
* `analysis_slug` - _required_ - Analysis' identifier

### Return crawl statistics grouped by time frequency (1 min, 5 mins or 60 min)

> Return crawl statistics grouped by time frequency (1 min, 5 mins or 60 min) for an analysis

*Tags:* `Analysis`

#### Input Parameters
* `limit` - _optional_ - max number of elements to retrieve
* `frequency` - _required_ - Aggregation frequency
    Possible values: 1mn, 5mn, 60mn.
* `analysis_slug` - _required_ - Analysis' identifier

### Return a list of 1000 latest URLs crawled (all crawled URLs or only URLS with HTTP errors)

*Tags:* `Analysis`

#### Input Parameters
* `username` - _required_ - User's identifier
* `project_slug` - _required_ - Project's identifier
* `analysis_slug` - _required_ - Analysis' identifier
* `list_type` - _required_ - URLs list type (crawled URLs or error URLs)
    Possible values: crawled, errors.

### List of Orphan URLs

> Legacy    List of Orphan URLs. URLs which generated visits from the selected source according to Google Analytics data, but were not crawled with by the Botify crawler (either because no links to them were found on the website, or because the crawler was not allowed to follow these links according to the project settings).   For a search engine (medium: origanic; sources: all, aol, ask, baidu, bing, google, naver, yahoo, yandex) or a social network (medium: social; sources: all, facebook, google+, linkedin, pinterest, reddit, tumblr, twitter)

*Tags:* `Analysis`

#### Input Parameters
* `page` - _optional_ - Page Number
* `size` - _optional_ - Page Size
* `analysis_slug` - _required_ - Analysis' identifier
* `medium` - _required_ - Type of traffic, value: 'organic' (from search engine)or 'social' (from a social network)
    Possible values: organic, social.
* `source` - _required_ - Traffic source, value: name of the search engine or social network
    Possible values: all, aol, ask, baidu, bing, facebook, google, google+, linkedin, naver, pinterest, reddit, tumblr, twitter, yahoo, yandex.

### Get inlinks percentiles

*Tags:* `Analysis`

#### Input Parameters
* `username` - _required_ - User's identifier
* `project_slug` - _required_ - Project's identifier
* `analysis_slug` - _required_ - Analysis' identifier

### Lost pagerank

*Tags:* `Analysis`

#### Input Parameters
* `username` - _required_ - User's identifier
* `project_slug` - _required_ - Project's identifier
* `analysis_slug` - _required_ - Analysis' identifier

### List clicks and impressions per day

*Tags:* `Analysis`

#### Input Parameters
* `username` - _required_ - User's identifier
* `project_slug` - _required_ - Project's identifier
* `analysis_slug` - _required_ - Analysis' identifier

### Get global information of the sitemaps found (sitemaps indexes, invalid sitemaps urls, etc

> Get global information of the sitemaps found (sitemaps indexes, invalid sitemaps urls, etc.)

*Tags:* `Analysis`

#### Input Parameters
* `username` - _required_ - User's identifier
* `project_slug` - _required_ - Project's identifier
* `analysis_slug` - _required_ - Analysis' identifier

### Sample list of URLs which were found in your sitemaps but outside of the

> Sample list of URLs which were found in your sitemaps but outside of the crawl perimeter defined for the project, for instance domain/subdomain or protocol (HTTP/HTTPS) not allowed in the crawl settings.

*Tags:* `Analysis`

#### Input Parameters
* `page` - _optional_ - Page Number
* `size` - _optional_ - Page Size
* `analysis_slug` - _required_ - Analysis' identifier

### Sample list of URLs which were found in your sitemaps, within the project

> Sample list of URLs which were found in your sitemaps, within the project allowed scope (allowed domains/subdomains/protocols), but not found by the Botify crawler.

*Tags:* `Analysis`

#### Input Parameters
* `page` - _optional_ - Page Number
* `size` - _optional_ - Page Size
* `analysis_slug` - _required_ - Analysis' identifier

### Top domains

*Tags:* `Analysis`

#### Input Parameters
* `page` - _optional_ - Page Number
* `size` - _optional_ - Page Size
* `analysis_slug` - _required_ - Analysis' identifier

### Top subddomains

*Tags:* `Analysis`

#### Input Parameters
* `page` - _optional_ - Page Number
* `size` - _optional_ - Page Size
* `analysis_slug` - _required_ - Analysis' identifier

### List of Orphan URLs

> List of Orphan URLs. URLs which generated visits from the selected source according to Google Analytics data, but were not crawled with by the Botify crawler (either because no links to them were found on the website, or because the crawler was not allowed to follow these links according to the project settings).   For a search engine (medium: origanic; sources: all, aol, ask, baidu, bing, google, naver, yahoo, yandex) or a social network (medium: social; sources: all, facebook, google+, linkedin, pinterest, reddit, tumblr, twitter)

*Tags:* `Analysis`

#### Input Parameters
* `page` - _optional_ - Page Number
* `size` - _optional_ - Page Size
* `analysis_slug` - _required_ - Analysis' identifier
* `medium` - _required_ - Type of traffic, value: 'organic' (from search engine)or 'social' (from a social network)
    Possible values: organic, social.
* `source` - _required_ - Traffic source, value: name of the search engine or social network
    Possible values: all, aol, ask, baidu, bing, facebook, google, google+, linkedin, naver, pinterest, reddit, tumblr, twitter, yahoo, yandex.

### Get the segments feature public metadata of an analysis

> Get the segments feature public metadata of an analysis.

*Tags:* `Analysis`

#### Input Parameters
* `page` - _optional_ - Page Number
* `size` - _optional_ - Page Size
* `analysis_slug` - _required_ - Analysis' identifier

### Return a list of all robots

> Return a list of all robots.txt files found on the project's domains.

*Tags:* `Analysis`

#### Input Parameters
* `page` - _optional_ - Page Number
* `size` - _optional_ - Page Size
* `analysis_slug` - _required_ - Analysis' identifier

### Return content of a robots

> Return content of a robots.txt file.

*Tags:* `Analysis`

#### Input Parameters
* `page` - _optional_ - Page Number
* `size` - _optional_ - Page Size
* `analysis_slug` - _required_ - Analysis' identifier
* `robots_txt` - _required_ - Filename

### Executes a query and returns a paginated response

*Tags:* `Analysis`

#### Input Parameters
* `area` - _optional_ - Analysis context
    Possible values: current, disappeared, new, search_engines_orphans, gsc_keywords, gsc_keywords_by_country.
* `page` - _optional_ - Page Number
* `size` - _optional_ - Page Size
* `previous_crawl` - _optional_ - Previous analysis identifier

### Query aggregator

> Query aggregator. It accepts multiple queries and dispatches them on ES or BQ.

*Tags:* `Analysis`

#### Input Parameters
* `area` - _optional_ - Analysis context
    Possible values: current, disappeared, new, search_engines_orphans, gsc_keywords, gsc_keywords_by_country.
* `previous_crawl` - _optional_ - Previous analysis identifier
* `analysis_slug` - _required_ - Analysis' identifier

### Gets an Analysis datamodel

*Tags:* `Analysis`

#### Input Parameters
* `area` - _optional_ - Analysis context
    Possible values: current, disappeared, new, search_engines_orphans, gsc_keywords, gsc_keywords_by_country.
* `previous_crawl` - _optional_ - Previous analysis identifier
* `analysis_slug` - _required_ - Analysis' identifier

### Gets Analysis Datasets

*Tags:* `Analysis`

#### Input Parameters
* `area` - _optional_ - Analysis context
    Possible values: current, disappeared, new, search_engines_orphans, gsc_keywords, gsc_keywords_by_country.
* `previous_crawl` - _optional_ - Previous analysis identifier
* `deprecated_fields` - _optional_ - Include deprecated fields

### A list of the CSV Exports requests and their current status

*Tags:* `Analysis`

#### Input Parameters
* `page` - _optional_ - Page Number
* `size` - _optional_ - Page Size
* `analysis_slug` - _required_ - Analysis' identifier

### Creates a new UrlExport object and starts a task that will export the results into a csv

> Creates a new UrlExport object and starts a task that will export the results into a csv. Returns the model id that manages the task

*Tags:* `Analysis`

#### Input Parameters
* `area` - _optional_ - Analysis context
    Possible values: current, disappeared, new, search_engines_orphans, gsc_keywords, gsc_keywords_by_country.
* `previous_crawl` - _optional_ - Previous analysis identifier
* `export_size` - _optional_ - Maximum size of the export (deprecated => size instead)
* `size` - _optional_ - Maximum size of the export

### Checks the status of an CSVUrlExportJob object

> Checks the status of an CSVUrlExportJob object. Returns json object with the status.

*Tags:* `Analysis`

#### Input Parameters
* `username` - _required_ - User's identifier
* `project_slug` - _required_ - Project's identifier
* `analysis_slug` - _required_ - Analysis' identifier
* `url_export_id` - _required_ - Url Export ID

### Gets the HTML of an URL for an analysis

*Tags:* `Analysis`

#### Input Parameters
* `username` - _required_ - User's identifier
* `project_slug` - _required_ - Project's identifier
* `analysis_slug` - _required_ - Analysis' identifier
* `url` - _required_ - (Urlencoded) Searched URL

### Return most frequent segments (= suggested patterns in the previous version)

> Return most frequent segments (= suggested patterns in the previous version) for a Botify Query.

*Tags:* `Analysis`

#### Input Parameters
* `area` - _optional_ - Analysis context
    Possible values: current, new.
* `project_slug` - _required_ - Project's identifier
* `analysis_slug` - _required_ - Analysis' identifier

### Gets the detail of an URL for an analysis

*Tags:* `Analysis`

#### Input Parameters
* `fields` - _optional_ - comma separated list of fields to return (c.f. URLs Datamodel)
* `project_slug` - _required_ - Project's identifier
* `analysis_slug` - _required_ - Analysis' identifier
* `url` - _required_ - (Urlencoded) Searched URL

### List all active projects for the user

*Tags:* `User`

#### Input Parameters
* `name` - _optional_ - Project's name
* `page` - _optional_ - Page Number
* `size` - _optional_ - Page Size

### Creates a new JobAutomation from data

*Tags:* `JobAutomation`

#### Input Parameters
* `username` - _required_ - user to which belongs the project
* `project_slug` - _required_ - identifies the project

### Creates a new JobAutomation from an existing job

*Tags:* `JobAutomation`

#### Input Parameters
* `username` - _required_ - user to which belongs the project
* `project_slug` - _required_ - identifies the project
* `job_id` - _required_ - the id of the existing job

### List all collections for a project

*Tags:* `Collections`

#### Input Parameters
* `username` - _required_ - User's identifier
* `project_slug` - _required_ - Project's identifier

### Get the detail of a collection

*Tags:* `Collections`

#### Input Parameters
* `username` - _required_ - User's identifier
* `project_slug` - _required_ - Project's identifier
* `collection` - _required_ - The collection to query

### List all datasources for a project

*Tags:* `Project`

#### Input Parameters
* `username` - _required_ - User's identifier
* `project_slug` - _required_ - Project's identifier

### List all the project's saved filters (each filter's name, ID and filter value)

*Tags:* `Project`

#### Input Parameters
* `username` - _required_ - User's identifier
* `project_slug` - _required_ - Project's identifier

### Retrieves a specific saved filter's name, ID and filter value

*Tags:* `Project`

#### Input Parameters
* `username` - _required_ - User's identifier
* `project_slug` - _required_ - Project's identifier
* `identifier` - _required_

### Project Query aggregator

> Project Query aggregator. It accepts multiple queries that will be executed on all completed analyses in the project

*Tags:* `Project`

#### Input Parameters
* `area` - _optional_ - Analyses context
    Possible values: current, disappeared, new, gsc_keywords, gsc_keywords_by_country.
* `last_analysis_slug` - _optional_ - Last analysis on the trend
* `nb_analyses` - _optional_ - Max number of analysis to return

### List all active projects for the user

*Tags:* `Project`

#### Input Parameters
* `username` - _required_ - User's identifier

## License

**flow**ground :- Telekom iPaaS / botify-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
