## ElasticSuite CMS Pages Search

This module is a plugin for [ElasticSuite](https://github.com/Smile-SA/elasticsuite).

It allows to index CMS Pages into the search engine and display them into the autocomplete results, and also on the search result page.

### ⚠️ Magento versions compatibility :

**Which version should I use ?**

Magento Version                                     | Module Version
----------------------------------------------------|------------------------------------------------------------------------
Magento **2.0.x** Opensource (CE) / Commerce (EE)   |**2.0.x** latest release : ```composer require smile/module-elasticsuite-cms-search ~2.0.0```
Magento **2.1.x** Opensource (CE) / Commerce (EE)   |**2.1.x** latest release : ```composer require smile/module-elasticsuite-cms-search ~2.1.0```
Magento **2.2.x** Opensource (CE) / Commerce (EE)   |**2.1.x** latest release : ```composer require smile/module-elasticsuite-cms-search ~2.1.0```

### Requirements

The module requires :

- [ElasticSuite](https://github.com/Smile-SA/elasticsuite) > 2.1.*

### How to use

1. Install the module via Composer :

``` composer require smile/module-elasticsuite-cms-search ```

2. Enable it

``` bin/magento module:enable Smile_ElasticsuiteCms ```

3. Install the module and rebuild the DI cache

``` bin/magento setup:upgrade ```

4. Process a full reindex of the CMS Page search index

``` bin/magento index:reindex elasticsuite_cms_page_fulltext ```

