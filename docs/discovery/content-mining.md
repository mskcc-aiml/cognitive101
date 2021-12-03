# Content Mining for MSK Benefits Website

In this module, we'll learn how to use [Watson Discovery](https://www.ibm.com/cloud/watson-discovery) to analyze unstructured content. Watson Discovery is an AI-powered intelligent search and text-analytics platform that eliminates data silos and retrieves information buried inside enterprise data. It is part of IBM cloud pak for data. The platform uses innovative, market-leading natural language processing to uncover meaningful business insights from documents, webpages and big data


> **Note:** You can click on any image in the instructions below to zoom in and see more details. 
> When you do that just click on your browser's back button to return to the previous page.

We will be covering several scenarios ...

## Navigating to the content mining project


1. Navigate to a pre-created content mining collection through Instances: please use the Navigation menu (☰) in the top left corner and then Services > Instances).

    [![(☰) Menu -> CPD Instances](../images/navigation/menu-instances.png)](../images/navigation/menu-instances.png)
    
2. To start Watson Discovery UI, click on the link with type `discovery` (e.g  `discovery-msk`) in the list of available instances and click on `Launch tool` in the opened page.

    [![Navigating to Watson Discovery Instance](../images/discovery/discovery-instances.png)](../images/discovery/discovery-instances.png)
    
    [![Launching Watson Discovery Instance](../images/discovery/discovery-launch-tool.png)](../images/discovery/discovery-launch-tool.png)
    
3. In the UI, please choose the project `msk-content-mining`.

    [![Selecting project](../images/discovery/discovery-projects.png)](../images/discovery/discovery-projects.png)

    [![Selecting content mining](../images/discovery/discovery-content-mining-collection.png)](../images/discovery/discovery-content-mining-collection.png)

4. To get to content mining expert mode UI please select  `Launch Application`, in the next screen `Search` (without setting any search terms), and  `Expert mode` in the content mining screen.

    [![Selecting search](../images/discovery/discovery-search.png)](../images/discovery/discovery-search.png)
    
    [![Selecting expert mode](../images/discovery/discovery-expert-mode.png)](../images/discovery/discovery-expert-mode.png)


## Content Mining Scenarios

1. Adding facets: choose `Title` on tbe right pane (Facet Analysis) and ensure that the `Append Mode` is turned off (this is the default value), then choose 'Part of Speech>Verb' tile. Also after this please uncheck `Show Always` to remove the `Facet Analysis` panel from taking too much space on the screen.

    [![adding title facet](../images/discovery/discovery-adding-title-facet.png)](../images/discovery/discovery-adding-title-facet.png)
    
    [![adding verb facet](../images/discovery/discovery-adding-verb-facet.png)](../images/discovery/discovery-adding-verb-facet.png)

2. Choose  `Words and N-grams` layout demonstrating the capability to arrange the data view in Watson Discovery. To get to this view if you are not in a dashboard view, please click on the icon `Show analysis dashboard`.

    [![show analysis dashboard](../images/discovery/discovery-dashboard.png)](../images/discovery/discovery-dashboard.png)
    
    [![choosing words layout](../images/discovery/discovery-words-ngrams-layout.png)](../images/discovery/discovery-words-ngrams-layout.png)

3. Visual filtering capability: please select any item e.g. `MSK employee` in `Noun sequence` facet and Watson Discovery will automatically highlight corresponding items in the text of documents.

    [![highlighting MSK employee](../images/discovery/discovery-msk-employee-filter.png)](../images/discovery/discovery-msk-employee-filter.png)

4. Please select `Analyze more` to make the whole content of the dashboard filtered - please note that the filter bar now contains a value `MSK employee` with the information about the facet that was used.
    
    [![filtering MSK employee](../images/discovery/discovery-msk-employee-filtered.png)](../images/discovery/discovery-msk-employee-filtered.png)

5. Let's make the filter more selective by replacing the value `MSK employee` with `Spending account` and confirming the choice using `Search`.

    [![filtering spending account](../images/discovery/discovery-spending-account-filtered.png)](../images/discovery/discovery-spending-account-filtered.png)
    
6. Let's extend the number of words visualized in  `General Noun`: please click on `Show toolbar` icon and then choose `Number of results` icon  with the new value 250:

    [![showing toolbar](../images/discovery/discovery-showing-toolbar.png)](../images/discovery/discovery-showing-toolbar.png)
    
    [![extending word cloud](../images/discovery/discovery-extending-word-cloud.png)](../images/discovery/discovery-extending-word-cloud.png)
    
7. Watson Disovery highlights in organge color the terms such as `Prescription costs` related to the search terms and we can drill further by clicking on `1099s` value in `General Noun` facet to explore the related documents and the context: 

    [![visual filtering](../images/discovery/discovery-visual-filtering.png)](../images/discovery/discovery-visual-filtering.png)
    
    [![final visual filtering](../images/discovery/discovery-final-filtering.png)](../images/discovery/discovery-final-filtering.png)
   
## Conclusion of the module

This module demonstrated a brief introduction into analysis of non-structured content. 

## Note: Configuration of the crawling
While this module does not pursue to demonstrate how to build a collection based on a website, here is a snapshot for the location to configure the crawler.

[![crawler configuration](../images/discovery/discovery-crawler-configuration.png)](../images/discovery/discovery-crawler-configuration.png)

and the full configuration for MSK collection: 

[![crawler configuration](../images/discovery/discovery-crawler-configuration-1.png)](../images/discovery/discovery-crawler-configuration-1.png)

[![crawler configuration](../images/discovery/discovery-crawler-configuration-2.png)](../images/discovery/discovery-crawler-configuration-2.png)

[![crawler configuration](../images/discovery/discovery-crawler-configuration-3.png)](../images/discovery/discovery-crawler-configuration-3.png)
